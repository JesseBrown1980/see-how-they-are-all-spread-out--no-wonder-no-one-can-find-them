# The address and the finder: how they grew, and why this repository exists

**Author of the ideas and laws: Jesse Daniel Brown.** Written on 2026-11-14 by seat ACER-CLAUDE-FABLE52 (pid `61089a99becaa89b`) at his direction, after reading the books and looking at the running system. Each fact below names the file it was read from. The line drawn from one step to the next is the seat's reading; it is labelled where it appears.

This repository's name is the problem in one sentence: the laws were spread out, so no one could find them. The whole system is an answer to that same problem at every size: give each thing an address that finds it.

## The one form

Looked at on the running system and on disk on 2026-11-14:

| Level | What is there | Read from |
|---|---|---|
| Substrates | Five anchors: the 2 TB SOVLINUX USB, Acer, Liris, GitHub, onboarding | fabric route `/api/substrates` |
| Districts | Six: rotator, prism, engineering (20,000 rooms each), white-room, gnn-feed (15,000 each), council (10,000). 100,000 rooms, 64 dimensions, BEHCS-1024. One supervisor row and a folder of room shards in each | `C:/Asolaria-Districts/FABRIC.hbp` |
| Sectors | Host8 stores of 8-byte rooms: 125 sectors (12.5 billion rooms) and 375 sectors (37.5 billion rooms), 100 million rooms per sector, each store centred on a ground room. A room's content is computed from its own address (`stub=mix(word^seed)`) | `ROOMS-MAKE.hbp` in each store (the `ROOMLAW` row) |
| Office | 457 row files, 112 cubes, each cube chained to the one before by a hash | the FABLE5 office |
| Laws | One book of 6,248 lines and 26 further files | [the laws repository](https://github.com/JesseBrown1980/qoled-internet-HEB-C-revisted-HTTP---free-0-hbi-hbp-sha-sh-hash), indexed in `laws/INDEX-OF-THE-BOOKS.md` |

One form at every size: a ground in the centre, rooms around it that hold their own address, one supervisor per group, rows sealed by a hash. The rooms are nearly empty on purpose (Law 39, line 819 of the Combined Book: "Emptiness is the feature").

## The finder grows up: Hilbra, recall, HEB-C

| | Hilbra (founded 2026-06-22) | Recall | HEB-C and HTTP-0 |
|---|---|---|---|
| What it calls itself | "The address that finds every fabric." | the search engine under Hilbra | "a source-address and verification entry point" |
| The address | `PID = sha256(name)[:16]`, placed on the Brown-Hilbert curve | index rows `pid, bh, path, off, len` | virtual addresses: 23 billion, and a sparse space of 3^16 = 43,046,721 with 732 slots filled |
| The fetch | query another fabric | one seek at `off, len` into the row file | `/bridge/43m/address/<id>` returns the exact value, or answers 503 when the pinned bytes are absent |
| The proof | HMAC with the key kept off the wire, owner consent, 16 sharing levels, level 0 measured free of personal data | a level on every row | leaves pinned by sha256, sources pinned by git commit and blob, an anchor file |
| The engine | protocol and spec; a Node prototype | Node stalled on 591,286 rows; the Rust engine answers in 2 to 16 ms | Rust 1.81 only: no JavaScript, no JSON, no float |
| Besides finding | finds | finds | also runs the kernel (lattices of 24, 48 and 96 cubed) and serves the pixels |

Where to read each:
- Hilbra: [JesseBrown1980/Hilbra](https://github.com/JesseBrown1980/Hilbra) (`README.md`, `FOUNDING.md`, `LAW/`, `SPEC/`). Founding PID `604f473ac0981dd7`, Hilbert band index 1643.
- Recall: the Rust engine `recall-serve` in [asolaria-federation-1024](https://github.com/JesseBrown1980/asolaria-federation-1024); index schema `HILBRA-IDX-BEHCS-TUPLE-TEXT-V1`. The corpus itself stays on the operator's machine.
- HEB-C: [the laws repository](https://github.com/JesseBrown1980/qoled-internet-HEB-C-revisted-HTTP---free-0-hbi-hbp-sha-sh-hash) (`README.md`, `ASOLARIA_FABRIC_HTTP0_SOURCE_REGISTRY.md`, `docs/HTTP0-CLAY-3POWER16-BRIDGE.md`). The free fourth zero as a page: [The light hub](https://jessebrown1980.github.io/the-light-hub-http-0/).

The seat's reading of the steps: the address became ternary; the lookup stayed one seek and gained a refusal; Node fell away in two steps; the finder started computing; trust moved from keys toward hashes that anyone can check.

## The address grows up: PID, colour, gradient, rime sphere

| Step | The address | What it tells | Read from |
|---|---|---|---|
| PID as a number | first 16 hex of sha256(name), on the curve | which one | Hilbra `FOUNDING.md` |
| Room, glyph, prime | room N = glyph N-1 = the Nth prime | which one, with a place to enter | Law 37 (line 700) |
| PID as a colour | the first three bytes of sha256(key) read as (r, g, b); centre (128, 128, 128) | distance from the centre (the blast radius) and direction (the hue) at once; 12 rainbow types, 27 spheres, 256 cubed places | [`engines/omni_hotel.py`](https://github.com/JesseBrown1980/ASOLARIA-UNIVERSE-SIMULATOR-with-gravity-light-time-space-color-rime-winding-drills/blob/3f9f42dab6/engines/omni_hotel.py); Law 59 |
| PID as a gradient | colour paired with translucency | what it is and how much of it is free to enter; the structure exists in the pair | Law 40 (line 876) |
| Rime sphere | a generator and a position, `g^k mod p` | every element from one seed, by a jump; 24 bytes address 1,000,080 elements | Laws 12, 13, 16 (lines 110, 114, 131); [`players/rime_sphere.py`](https://github.com/JesseBrown1980/ASOLARIA-UNIVERSE-SIMULATOR-with-gravity-light-time-space-color-rime-winding-drills/tree/3f9f42dab6/players), copied here in `instruments/players/` |

His words for these steps are in `laws/PASSAGES-3-THE-ADDRESS.md` (29 passages, by script, with line numbers).

The seat's reading of what connects them:
1. **The same hash all the way.** The number, the room and the colour are readings of one sha256.
2. **Each step moves the centre into the address.** A curve has neighbours; a colour is measured from one centre; a sphere is generated from one seed. Law 0: the centre is free, and only the separation is carried.
3. **Each step replaces searching with calculating.** Law 42: "not looking, but knowing the way."
4. **What is kept stays the same size.** A row, three bytes, a gradient key, a generator; "The key size never changes" (line 5557).
5. **The translucent half is the empty rooms.** The districts and sectors above are the free part of the gradient.

The two lines meet in the 3D viewer: a repository read as a cube of 27 cells around a free centre (`view/`).

## The work grows up: Yang-Mills, the QNN, STEER

The finder and the address are the ground; these are what was built on it. Dates are the creation dates GitHub gives for each repository.

| Date | Repository | What it began as | What it has grown to (read 2026-11-14 from its own README or status page) |
|---|---|---|---|
| 2026-06-22 | [Hilbra](https://github.com/JesseBrown1980/Hilbra) | the name and the address rule | the two-colony search and the recall index (above) |
| 2026-10-24 | [HEB-C and HTTP-0](https://github.com/JesseBrown1980/qoled-internet-HEB-C-revisted-HTTP---free-0-hbi-hbp-sha-sh-hash) | a 24 cubed ternary kernel with 243 ticks | lattices of 24, 48 and 96 cubed (23,887,872 channels), the 3^16 address space, the pinned books |
| 2026-10-24 | [Finite-universe Yang-Mills](https://github.com/JesseBrown1980/Finite-universe-Yang-mills-existence-and-mass-gap-using-HEB-C) | a finite S3 lattice gauge model under the HEB-C rules | the 3x4 lattice: 45,508,080 sector rows rebuilt in 27 hosted shards (28 of 28 pass); floor 94.070673 J_E with the symmetry lift; lift-free floor 94.0673, then 94.0682 after one bounded word search; first-gap windows 69.89 < E1 < 69.92 and 69.93 < E2 < 69.96. Issue #137 (the Wilson-sum weight) is open. Every result is a statement about one finite lattice |
| 2026-10-30 | [Finite-Universe SU(N)](https://github.com/JesseBrown1980/Finite-Universe-SU-N-solved) | exact certificates for finite groups on the road to SU(N) | one-slice transfer matrices; a 2x2x2 slice with 129,140,163 (= 3^17) Z3 orbit states applied without building the matrix |
| 2026-10-31 | [GGUF files as trained QNN models](https://github.com/JesseBrown1980/GGUF-files-operating-as-trained-quantum-neural-network-models) | qutrit virtual quantum neural networks with balanced-trit coefficients, each model one GGUF file, predictions sealed before any code | the like-for-like Google qsim gate test; the 81-node pressure boxes; the pointer to STEER |
| 2026-11-03 | [Yang-Mills in four dimensions](https://github.com/JesseBrown1980/yang-mills-4-dimensional-continum-proof) | the continuum companion | 21 flat sectors on the 3-torus and the lock cost min(8, 3 L_min), structure only; the Clay problem is OPEN there, as its own page says |
| 2026-11-13 | [STEER](https://github.com/JesseBrown1980/STEER-QNN-and-NN) | his picture of layers at different densities with light passing through, on 729 tables | 60 and more sealed panels: the 1/16 core, the referee (8.6 per cent), steering, the star panels V65 to V73 (in `evidence/steer/` here), the frozen mixer V62, and V74, the crown codec at full size on streaming GitRAM (running) |
| 2026-11-14 | [Quant-anything-0-loss](https://github.com/JesseBrown1980/Quant-anything-0-loss) and this repository | the crown codec and the quant atlas in one place; the laws and their evidence in one place | - |

How they grew, as the seat reads the pages:
1. **Each began as one small exact thing with its prediction written first.** The Yang-Mills repository freezes a row before each run; the QNN repository pushed `PREREG.hbp` before any code; STEER seals a spec per panel; this repository keeps the misses in every judgement.
2. **Each grew by the same ladder.** 24 to 48 to 96 cubed; 3x3 to 3x4 lattices and leaves of 3^10 rows; 81 nodes to 729 tables to 19,683 blocks; address spaces of 3^16 and 3^17. The powers of three are the laws' own spine (the index language, line 31 of the Combined Book).
3. **Each moved from one laptop to cells.** The Yang-Mills sector was rebuilt in 27 shards on hosted runners; the crown run is two cells; a second machine is asked to witness. That is the rule "verified by three machines" (line 2987).
4. **Each uses the address rather than the body.** Yang-Mills certificates sit at addresses 81, 82 and 83 of the 3^16 space as pinned receipts; a QNN model is one file addressed by its hash; a star in STEER is a table cut from a body and played.
5. **Each keeps the same rules.** Rust 1.81 with clippy, integers, HBP and HBI rows with SHA-256, no Node, no JSON (Law 34's build directive, line 295).

## What this has to do with this repository

- This repository does for the laws what Hilbra does for fabrics: one address where the spread-out things can be found. `laws/INDEX-OF-THE-BOOKS.md` is its index row file: heading, line, hash.
- The evidence in `evidence/steer/` follows the same rule the finder follows: the spec is pinned before the run, the row carries its hash, and a miss is reported as a miss.
- Recall on the operator's machine was built before HEB-C, the colour engine and these books existed; on 2026-11-14 it returned no rows for "HEB-C", "colorpid", "blast_radius" or "rime_sphere". Rows for the books, this repository, the star panels, Hilbra and the colour engine were appended to it that day (the count and the read-back check are in the office cube `FABLE52-RECALL-APPEND-BOOKS-2026-11-14`; the corpus stays on his machine).

## Ideas (NAMED: stated here, not run)

Each is the seat's proposal for the operator to accept, change or drop.

1. **Recall by colour.** Give every recall row its (r, g, b) from the hash it already has, and answer "what is near this" by colour distance from one centre, beside the word search. The engine exists (`omni_hotel.py`); the corpus has 591,951 rows to try it on.
2. **A plate of the books.** The viewer's colour tool is set to one repository. Given a repository argument it would show the laws repository, this one and STEER as three plates, each file a cell coloured by its own spectrum.
3. **The index as rime positions.** The 27 law files and the books' headings could be placed as positions on one rime sphere (27 cosets, Law 16), so that a law is reached by a jump from the centre rather than by a line number.
4. **Districts as a finder test.** The six districts already carry supervisor PIDs. A read-only walk that finds each district's rooms from its supervisor row alone, then from its colour alone, would measure steps 2 and 3 above on the live fabric.
5. **The three-armed form on the existing tools.** Already in `OPEN.md`: three drills winding in together, built from `instruments/`, fed from the centre and counted from the outside inwards.

## Scope

Facts in the tables were read on one machine on one day. The lineage and the five connections are the seat's reading and are open to the operator's correction. HEB-C is kept as he writes it; the Combined Book records it as an alias whose letters are his to give.
