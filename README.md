## aui-perf nightly record

_4 points · 2026-11-15T12:05:47.933Z to 2026-11-19T13:16:45.707Z · latest runner: AMD EPYC 9V74 80-Core Processor · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 705.32µs |  |  | 544.60µs | 705.32µs | 4 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 1.009ms |  |  | 769.48µs | 1.009ms | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 45.43µs |  |  | 33.07µs | 46.13µs | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 524.26µs |  |  | 377.19µs | 539.46µs | 4 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 8.174ms |  |  | 5.782ms | 8.399ms | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 222.31µs |  |  | 153.69µs | 226.52µs | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.108ms |  |  | 1.420ms | 2.204ms | 4 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 8.128ms |  |  | 5.682ms | 8.300ms | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 8.32µs |  |  | 6.24µs | 8.32µs | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 69.91µs |  |  | 52.78µs | 69.91µs | 4 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 274.29µs |  |  | 207.03µs | 274.29µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 81.28µs |  |  | 54.34µs | 81.28µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 43.90µs |  |  | 30.01µs | 43.90µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 43.49µs |  |  | 31.40µs | 43.49µs | 4 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 257.95µs |  |  | 190.24µs | 257.95µs | 4 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 53.49µs |  |  | 44.23µs | 56.17µs | 4 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 532.94µs |  |  | 467.94µs | 555.41µs | 4 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 7.60µs |  |  | 6.08µs | 7.88µs | 4 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 61.83µs |  |  | 51.77µs | 61.97µs | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 594.84µs |  |  | 436.16µs | 594.84µs | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 5.111ms |  |  | 3.676ms | 5.111ms | 4 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 20.103ms |  |  | 14.345ms | 20.103ms | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 289.67µs |  |  | 202.62µs | 289.67µs | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.836ms |  |  | 1.982ms | 2.836ms | 4 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 11.300ms |  |  | 7.875ms | 11.300ms | 4 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 220.52µs |  |  | 202.43µs | 228.24µs | 4 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.683ms |  |  | 1.260ms | 1.852ms | 4 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 50.66µs |  |  | 41.63µs | 52.70µs | 4 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 508.08µs |  |  | 409.34µs | 508.08µs | 4 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.697ms |  |  | 2.202ms | 2.697ms | 4 |
| external-message-conversion › core: external message tool results › 100 matches | 59.31µs |  |  | 52.50µs | 61.57µs | 4 |
| external-message-conversion › core: external message tool results › 1000 matches | 601.39µs |  |  | 521.25µs | 619.87µs | 4 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.158ms |  |  | 2.769ms | 3.241ms | 4 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 31.28µs |  |  | 26.90µs | 32.37µs | 4 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 302.33µs |  |  | 257.78µs | 306.21µs | 4 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.618ms |  |  | 1.399ms | 1.618ms | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.21µs |  |  | 0.17µs | 0.21µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.37µs |  |  | 0.31µs | 0.37µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 2.11µs |  |  | 1.61µs | 2.11µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.50µs |  |  | 0.38µs | 0.50µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.47µs |  |  | 2.25µs | 2.47µs | 4 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 23.01µs |  |  | 20.05µs | 23.01µs | 4 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 115.56µs |  |  | 111.62µs | 127.24µs | 4 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 584.91µs |  |  | 584.91µs | 723.93µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.124ms |  |  | 1.942ms | 2.401ms | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 161.10µs |  |  | 118.01µs | 178.62µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.758ms |  |  | 2.508ms | 3.136ms | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 359.35µs |  |  | 335.14µs | 388.08µs | 4 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 504.65µs |  |  | 488.36µs | 575.52µs | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 6.105ms |  |  | 5.131ms | 6.964ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 759.74µs |  |  | 481.49µs | 827.62µs | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 16.410ms |  |  | 14.256ms | 17.044ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.785ms |  |  | 2.304ms | 2.785ms | 4 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.949ms |  |  | 1.722ms | 2.150ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.378ms |  |  | 1.952ms | 2.409ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.508ms |  |  | 2.171ms | 2.611ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 17.176ms |  |  | 13.319ms | 17.176ms | 4 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 18.437ms |  |  | 14.584ms | 18.437ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.001ms |  |  | 1.001ms | 1.298ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.143ms |  |  | 1.861ms | 2.360ms | 4 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 7.782ms |  |  | 6.351ms | 7.834ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.289ms |  |  | 1.241ms | 1.522ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.592ms |  |  | 1.294ms | 1.592ms | 4 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.257ms |  |  | 3.547ms | 4.685ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 258.53µs |  |  | 187.86µs | 258.53µs | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.215ms |  |  | 1.569ms | 2.215ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 215.085ms |  |  | 179.783ms | 224.856ms | 4 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 10.957ms |  |  | 7.717ms | 10.957ms | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.85µs |  |  | 1.18µs | 1.85µs | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 9.58µs |  |  | 5.32µs | 9.58µs | 4 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 36.17µs |  |  | 25.23µs | 36.17µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 7.32µs |  |  | 4.69µs | 7.32µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 19.86µs |  |  | 15.46µs | 19.86µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 72.38µs |  |  | 45.80µs | 72.38µs | 4 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 253.64µs |  |  | 187.10µs | 253.64µs | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 5.125ms |  |  | 4.083ms | 5.125ms | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 34.080ms |  |  | 24.093ms | 34.080ms | 4 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 393.525ms |  |  | 316.556ms | 393.525ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 515.57µs |  |  | 339.76µs | 515.57µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 702.52µs |  |  | 662.29µs | 771.71µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 4.229ms |  |  | 3.069ms | 4.229ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 527.16µs |  |  | 361.40µs | 527.16µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.254ms |  |  | 1.128ms | 1.254ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 15.962ms |  |  | 7.795ms | 15.962ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 489.32µs |  |  | 324.40µs | 489.32µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 909.32µs |  |  | 835.25µs | 909.32µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 10.255ms |  |  | 5.353ms | 10.255ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 243.00µs |  |  | 142.73µs | 243.00µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 483.41µs |  |  | 342.76µs | 483.41µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.637ms |  |  | 2.410ms | 2.815ms | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 13.74µs |  |  | 10.62µs | 13.74µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 27.70µs |  |  | 21.81µs | 27.70µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 203.25µs |  |  | 193.85µs | 224.66µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 467.53µs |  |  | 399.50µs | 467.53µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 877.67µs |  |  | 842.45µs | 934.56µs | 4 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 9.087ms |  |  | 5.697ms | 9.087ms | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 204.93µs |  |  | 155.57µs | 204.93µs | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.824ms |  |  | 1.413ms | 1.824ms | 4 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 909.53µs |  |  | 717.37µs | 909.53µs | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 243.24µs |  |  | 171.32µs | 243.24µs | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 2.140ms |  |  | 1.513ms | 2.140ms | 4 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 1.081ms |  |  | 768.26µs | 1.081ms | 4 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 267.06µs |  |  | 242.40µs | 286.72µs | 4 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 21.404ms |  |  | 16.679ms | 21.404ms | 4 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 475.129ms |  |  | 475.129ms | 743.935ms | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 189.74µs |  |  | 125.86µs | 189.74µs | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.579ms |  |  | 1.053ms | 1.579ms | 4 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 810.92µs |  |  | 534.76µs | 810.92µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 163.52µs |  |  | 141.51µs | 169.79µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 763.54µs |  |  | 702.26µs | 794.84µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 178.67µs |  |  | 153.14µs | 187.24µs | 4 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 786.88µs |  |  | 725.54µs | 824.38µs | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.742ms |  |  | 2.198ms | 2.742ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.802ms |  |  | 2.263ms | 2.802ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.683ms |  |  | 2.192ms | 2.683ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.710ms |  |  | 2.152ms | 2.710ms | 4 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.715ms |  |  | 1.419ms | 1.782ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.525ms |  |  | 2.151ms | 2.640ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.539ms |  |  | 2.172ms | 2.539ms | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 200.41µs |  |  | 173.54µs | 227.10µs | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 108.60µs |  |  | 94.45µs | 108.60µs | 4 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.358ms |  |  | 1.136ms | 1.370ms | 4 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.427ms |  |  | 1.200ms | 1.505ms | 4 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.494ms |  |  | 1.284ms | 1.651ms | 4 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 38.98µs |  |  | 29.63µs | 38.98µs | 4 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 40.22µs |  |  | 31.58µs | 40.22µs | 4 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 53.95µs |  |  | 43.78µs | 60.03µs | 4 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.121ms |  |  | 952.68µs | 1.253ms | 4 |

informational; points come from different runners of the same class, so read trends, not single deltas.
