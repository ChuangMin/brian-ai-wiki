# Systems design and engineering fundamentals

[中文](../../docs/systems-design.md) | English

[Home](../index.md)

Non-AI backend and distributed-systems basics and operations (such as a TLS checkup), expected in a staff-engineer interview

### [12 systems-design basics](https://www.facebook.com/reel/3285768298275601)

A one-line lookup of 12 systems-design basics

| Credibility | Stars | Source |
| --- | --- | --- |
| — | — | [Video 22](https://www.facebook.com/reel/3285768298275601) |

A 13-second animated card from Code Crack (dark grid, 12 cards lighting up in order, no narration, made by hand, not AI-generated). Load balancer spreads traffic. Caching stores repeated queries. A CDN puts content closer to the user. Sharding splits data. Replication keeps copies for reads and failure. A message queue handles work asynchronously and reliably. Rate limiting caps traffic. Consistent hashing avoids reshuffling most keys when a node is added. CAP is consistency, availability, and partition tolerance. Idempotency means a retry does no extra harm. A circuit breaker stops a cascade. Observability uses logs, metrics, and traces to see the system. Correction: the chart's "pick two of three" for CAP is too simple. A partition is not optional. When a partition happens you choose between consistency and availability. With no partition, PACELC says the tradeoff is latency versus consistency. Music: UI sounds (a rising marimba and a closing chime) over a faint generic upbeat tech beat. Interview takeaway: an AI agent is a distributed system too. Retried tool calls must be idempotent, the LLM API needs a circuit breaker and a rate limit, long agent jobs go on a queue, and every agent run needs traces.

![On a dark grid, a 3×4 set of cards fades in. Each card has a small diagram (a split point, a cache block, shard bars) and a green frame highlights them in turn. Recreate it with CSS grid and staggered animation-delay.](../../assets/gifs/v22-system-design-cards.gif)

On a dark grid, a 3×4 set of cards fades in. Each card has a small diagram (a split point, a cache block, shard bars) and a green frame highlights them in turn. Recreate it with CSS grid and staggered animation-delay.

### [10 commands to check a site's HTTPS](https://www.facebook.com/reel/4523349764619784)

From certificate expiry and HSTS to old TLS: 10 commands for a quick HTTPS checkup

| Credibility | Stars | Source |
| --- | --- | --- |
| — | — | [Video 23](https://www.facebook.com/reel/4523349764619784) |

Code Crack (CodeCrackAI)'s animated terminal card "SECURITY • TLS FIRST AID". Sample output marks in red the certificate end date, TLSv1.0 still enabled, and `server: nginx/1.18.0` leaking the version. Made by hand, not AI-generated. Ten checks: `curl -sI` to see if it answers; `openssl s_client` to get the certificate; `openssl x509 -enddate` for the expiry; `-issuer` for the issuer; `-ext subjectAltName` for covered domains; whether HTTP uses `location` to redirect to HTTPS; whether `strict-transport-security` (HSTS) is present; `nmap --script ssl-enum-ciphers` for old protocols; whether the `server` header leaks a version; `dig CAA` for who may issue certificates. Correction: step 2 says "save as cert.pem", but the command itself does not save a file. It should be `echo | openssl s_client -connect example.com:443 -servername example.com 2>/dev/null | openssl x509 > cert.pem`, and `-servername` is required for SNI. A check of wiki.singularityengine.dev on 2026-10-31: HTTP/2 200; issued by Let's Encrypt (YR2), expiring 2027-01-29; the SAN is only wiki.singularityengine.dev; `server: GitHub.com`; but http:// returns a Cloudflare 500, does not redirect, and has no HSTS header. singularityengine.dev has no CAA record. Music: no voice and no music, only UI beeps and a closing chord. See also Security and governance. Interview takeaway: this kind of checklist should run in CI and monitoring (for example a certificate-expiry alert), not by hand. An AI agent can run it, but the result still passes a gate.

![The step list on the left advances with an orange highlight, the terminal on the right types commands and output, and risks are in red. Green lines flow in the background. Recreate it with a typewriter effect and an active class on the current step.](../../assets/gifs/v23-https-terminal-steps.gif)

The step list on the left advances with an orange highlight, the terminal on the right types commands and output, and risks are in red. Green lines flow in the background. Recreate it with a typewriter effect and an active class on the current step.

### [Handwritten-style Kafka architecture notes](https://www.facebook.com/reel/3443590945824757)

One handwritten-style note for the Kafka architecture (ZooKeeper is outdated)

| Credibility | Stars | Source |
| --- | --- | --- |
| — | — | [Video 25](https://www.facebook.com/reel/3443590945824757) |

A 15-second still from softwaredeveloper077, a digital handwritten note titled "KAFKA ARCHITECTURE" in 11 blocks: Producers; Cluster / Brokers; Consumers; Topics; Partitions (ordered, immutable, the source of parallelism); Replication (leader / followers); ZooKeeper; data flow (offset, commit); benefits; use cases; best practices (meaningful topic names, a sensible partition count, replicas, monitor consumer lag, retention by time and size, consumer groups, tune batch size). No watermark. The handwriting is clean and looks handmade, but AI cannot be ruled out completely. Correction: ZooKeeper is outdated. KRaft replaces it (production-ready since 3.3; ZooKeeper is removed in 4.0). Music: generic royalty-free upbeat electronic / house. Interview takeaway: a queue like Kafka can be the backbone of an event-driven agent pipeline. When you talk about Kafka, mention KRaft, so the knowledge is current.

### [Breadth-first search: how many steps to a crush](https://www.facebook.com/reel/1108544155324652)

Search outward through friends of friends, and see why BFS finds a shortest path

| Credibility | Stars | Source |
| --- | --- | --- |
| High credibility · small code bug | — | [Video 30](https://www.facebook.com/reel/1108544155324652) |

A BFS animation by thachdv.it (Vietnamese). The copy is 「Thuật toán tìm kiếm theo chiều rộng - BFS. Cách các nền tảng giúp b dò nhà crush 😁」 (BFS: how platforms help you find your crush's home). Concentric rings around YOU. Crush is on ring 4. Visited nodes light up. A QUEUE shows enqueue and dequeue (FIFO), plus CHECKED and RING counters. Steps: check friends, then friends of friends, one ring at a time. The queue stays first-in first-out. Stop at the first hit. The shortest path is marked "4 handshakes: the fewest there are". On-screen code: `queue, seen = deque([you]), {you}`, then `while queue: u = queue.popleft(); if u == crush: break; for v in friends[u]: if v not in seen: seen.add(v); came[v] = u; queue.append(v)`. Correctness: on an unweighted graph, BFS does give a shortest path (degrees of separation). Small bug: `came` is never initialized (it needs `came = {}` first). Copying it as shown raises NameError. The copy says "find the crush's home", but the video only covers handshake distance in a social graph. Real map routing has edge weights and needs Dijkstra or A*. Music: 8-bit chiptune, no narration. GIF segment: 0:00–0:11. Interview takeaway: unweighted graphs use BFS, weighted graphs use Dijkstra, and a heuristic uses A*. Uses include friend recommendations, "people you may know", and blast-radius analysis on a dependency graph.

![BFS expands ring by ring from YOU (nodes colored by layer). CHECKED and RING counters sit above. Code highlights line by line and QUEUE dots move in and out. The shortest path is marked in gold. Recreate it with SVG nodes, a step state machine, and line highlighting.](../../assets/gifs/v30-bfs-ring-expansion-queue.gif)

BFS expands ring by ring from YOU (nodes colored by layer). CHECKED and RING counters sit above. Code highlights line by line and QUEUE dots move in and out. The shortest path is marked in gold. Recreate it with SVG nodes, a step state machine, and line highlighting.

▶ Interactive demo: [Open](../../demos/bfs/) (https://wiki.singularityengine.dev/demos/bfs/)

### [Prim's algorithm: a minimum spanning tree](https://www.facebook.com/reel/2132850694107274)

Start at one node and always take the cheapest edge that leaves the tree, until every node is connected as cheaply as possible

| Credibility | Stars | Source |
| --- | --- | --- |
| High credibility | — | [Video 31](https://www.facebook.com/reel/2132850694107274) |

An animation by Software with John (copy: "Prim's Algorithm #dsa"). Undirected graph A–G. Edges: A-B 4, A-C 2, B-C 1, B-D 5, B-E 9, C-D 8, C-F 10, D-E 3, D-F 2, E-F 4, E-G 3, F-G 3. Starting at A, the picks are A-C(2), C-B(1), skip A-B(4) (B is already in the tree, so it would cycle, and it flashes red), B-D(5), D-F(2), D-E(3), F-G(3). Total weight 16. On-screen point: "Grow one tree outward from a start node, always taking the cheapest edge that leaves it." Code: Python `heapq`. Skip `v in seen`, then push neighboring edges onto the heap. Complexity is shown as time O(E log V) and space O(E). Correctness: checked. The sum 16 is a minimum spanning tree (Kruskal cross-checks to 16 as well). Look: dark background, heap edges are blue dashes, chosen edges glow cyan, rejected edges flash red. Music: unconfirmed (there was no audio track in the analysis). GIF segment: 0:02–0:07, including the red skip. Interview takeaway: Prim is a greedy algorithm based on the cut property. It grows a tree from one node with a heap. Kruskal sorts every edge and uses Union-Find. Dijkstra looks similar, but it compares accumulated distance, while Prim compares a single edge weight. Uses include lowest-cost network or wiring plans, and clustering.

![Prim's algorithm: starting at A, the cheapest edges join the tree as cyan solid lines. Candidate edges are dashed in the heap. Edges already in the tree are marked red and skipped. The code and the caption stay in step. Recreate it by switching SVG edge classes and stepping through a data array.](../../assets/gifs/v31-prim-mst-heap-edges.gif)

Prim's algorithm: starting at A, the cheapest edges join the tree as cyan solid lines. Candidate edges are dashed in the heap. Edges already in the tree are marked red and skipped. The code and the caption stay in step. Recreate it by switching SVG edge classes and stepping through a data array.

▶ Interactive demo: [Open](../../demos/prim/) (https://wiki.singularityengine.dev/demos/prim/)

### [Five GitHub repos every engineer should know](https://www.facebook.com/reel/1849291249414632) ⚠️

Five classic GitHub repos: rebuild tools yourself, learning roadmaps, systems design, free books, algorithms

![codecrafters-io/build-your-own-x GitHub preview](https://opengraph.githubassets.com/1/codecrafters-io/build-your-own-x)

![nilbuild/developer-roadmap GitHub preview](https://opengraph.githubassets.com/1/nilbuild/developer-roadmap)

![donnemartin/system-design-primer GitHub preview](https://opengraph.githubassets.com/1/donnemartin/system-design-primer)

![EbookFoundation/free-programming-books GitHub preview](https://opengraph.githubassets.com/1/EbookFoundation/free-programming-books)

![TheAlgorithms/Python GitHub preview](https://opengraph.githubassets.com/1/TheAlgorithms/Python)

| Credibility | Stars | Source |
| --- | --- | --- |
| ⚠️ engagement bait · high credibility | — | [Video 32](https://www.facebook.com/reel/1849291249414632) ⚠️ |

A real talking-head video by James Mcquay (the post says Comment "AI", and in the video he also asks viewers to comment "Github" so a private message can send the links; that is comment-driven engagement bait. Nothing is actually hidden: every repo name is spoken and subtitled). The on-screen line "10/10 GitHub repositories to make you an elite developer" is marketing exaggeration. (1) build-your-own-x (⚠️ https://github.com/codecrafters-io/build-your-own-x ⚠️): rebuild Git, Docker, databases, and so on from scratch, 557.8k stars (the video says 485k, which is out of date). (2) roadmap.sh (⚠️ https://github.com/nilbuild/developer-roadmap ⚠️, formerly kamranahmedse/developer-roadmap, renamed): learning roadmaps for backend, frontend, DevOps, and AI, 370.9k stars. (3) system-design-primer (⚠️ https://github.com/donnemartin/system-design-primer ⚠️): caching, load balancing, scalability, 376.3k stars. (4) free-programming-books (⚠️ https://github.com/EbookFoundation/free-programming-books ⚠️): free books and courses, 400.6k stars. (5) TheAlgorithms/Python (⚠️ https://github.com/TheAlgorithms/Python ⚠️): algorithm implementations, 225.7k stars. Stars checked 2026-10-31. Credibility: high. The repos are real classics. Only the "elite developer" line is inflated. Music: soft lo-fi background. A static talking head, no GIF clip. Interview takeaway: system-design-primer pairs with the other systems-design items in this category. build-your-own-x is a way to train fundamentals. In the era of AI-written code, a person still has to understand the lower layers to review that code.
