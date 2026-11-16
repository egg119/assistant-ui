## aui-perf nightly record

_2 points · 2026-11-15T12:05:47.933Z to 2026-11-16T12:54:54.335Z · latest runner: INTEL(R) XEON(R) PLATINUM 8573C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 615.53µs |  |  | 561.65µs | 615.53µs | 2 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 910.15µs |  |  | 796.55µs | 910.15µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 46.13µs |  |  | 35.82µs | 46.13µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 539.46µs |  |  | 387.30µs | 539.46µs | 2 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 8.399ms |  |  | 6.000ms | 8.399ms | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 226.52µs |  |  | 165.80µs | 226.52µs | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 2.204ms |  |  | 1.467ms | 2.204ms | 2 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 8.300ms |  |  | 5.951ms | 8.300ms | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 7.22µs |  |  | 6.50µs | 7.22µs | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 58.50µs |  |  | 53.67µs | 58.50µs | 2 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 230.24µs |  |  | 211.24µs | 230.24µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 71.50µs |  |  | 54.34µs | 71.50µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 35.37µs |  |  | 30.01µs | 35.37µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 35.33µs |  |  | 32.09µs | 35.33µs | 2 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 229.51µs |  |  | 192.21µs | 229.51µs | 2 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 56.17µs |  |  | 44.76µs | 56.17µs | 2 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 555.41µs |  |  | 489.41µs | 555.41µs | 2 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 7.88µs |  |  | 6.26µs | 7.88µs | 2 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 61.97µs |  |  | 53.20µs | 61.97µs | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 535.27µs |  |  | 436.64µs | 535.27µs | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 4.326ms |  |  | 3.677ms | 4.326ms | 2 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 16.767ms |  |  | 14.345ms | 16.767ms | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 253.34µs |  |  | 206.26µs | 253.34µs | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.568ms |  |  | 2.017ms | 2.568ms | 2 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 10.074ms |  |  | 7.875ms | 10.074ms | 2 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 228.24µs |  |  | 216.39µs | 228.24µs | 2 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.852ms |  |  | 1.838ms | 1.852ms | 2 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 52.70µs |  |  | 42.73µs | 52.70µs | 2 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 501.95µs |  |  | 422.31µs | 501.95µs | 2 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.618ms |  |  | 2.239ms | 2.618ms | 2 |
| external-message-conversion › core: external message tool results › 100 matches | 61.57µs |  |  | 54.08µs | 61.57µs | 2 |
| external-message-conversion › core: external message tool results › 1000 matches | 619.87µs |  |  | 541.08µs | 619.87µs | 2 |
| external-message-conversion › core: external message tool results › 5000 matches | 3.241ms |  |  | 2.843ms | 3.241ms | 2 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 32.37µs |  |  | 27.78µs | 32.37µs | 2 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 306.21µs |  |  | 272.52µs | 306.21µs | 2 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.604ms |  |  | 1.442ms | 1.604ms | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.19µs |  |  | 0.17µs | 0.19µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.35µs |  |  | 0.32µs | 0.35µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.92µs |  |  | 1.63µs | 1.92µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.47µs |  |  | 0.39µs | 0.47µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.47µs |  |  | 2.28µs | 2.47µs | 2 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 22.36µs |  |  | 20.05µs | 22.36µs | 2 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 127.24µs |  |  | 112.80µs | 127.24µs | 2 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 723.93µs |  |  | 641.55µs | 723.93µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 2.401ms |  |  | 1.953ms | 2.401ms | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 178.62µs |  |  | 118.16µs | 178.62µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 3.136ms |  |  | 2.559ms | 3.136ms | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 388.08µs |  |  | 349.05µs | 388.08µs | 2 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 575.52µs |  |  | 517.22µs | 575.52µs | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 6.964ms |  |  | 5.131ms | 6.964ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 827.62µs |  |  | 481.49µs | 827.62µs | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 17.044ms |  |  | 14.933ms | 17.044ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.726ms |  |  | 2.316ms | 2.726ms | 2 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 2.150ms |  |  | 1.795ms | 2.150ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.409ms |  |  | 2.033ms | 2.409ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.611ms |  |  | 2.274ms | 2.611ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 15.999ms |  |  | 13.955ms | 15.999ms | 2 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 17.704ms |  |  | 15.304ms | 17.704ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.298ms |  |  | 1.126ms | 1.298ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 2.360ms |  |  | 1.973ms | 2.360ms | 2 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 7.834ms |  |  | 6.684ms | 7.834ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.241ms |  |  | 1.241ms | 1.427ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.294ms |  |  | 1.294ms | 1.467ms | 2 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 4.685ms |  |  | 3.770ms | 4.685ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 256.26µs |  |  | 212.14µs | 256.26µs | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 2.178ms |  |  | 1.733ms | 2.178ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 224.856ms |  |  | 185.854ms | 224.856ms | 2 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 10.706ms |  |  | 8.461ms | 10.706ms | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.68µs |  |  | 1.19µs | 1.68µs | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 6.18µs |  |  | 5.40µs | 6.18µs | 2 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 28.63µs |  |  | 25.55µs | 28.63µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 5.75µs |  |  | 4.70µs | 5.75µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 16.86µs |  |  | 15.63µs | 16.86µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 55.29µs |  |  | 45.91µs | 55.29µs | 2 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 198.54µs |  |  | 190.67µs | 198.54µs | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 5.011ms |  |  | 4.470ms | 5.011ms | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 28.936ms |  |  | 26.825ms | 28.936ms | 2 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 355.301ms |  |  | 316.556ms | 355.301ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 399.30µs |  |  | 350.77µs | 399.30µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 771.71µs |  |  | 662.29µs | 771.71µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.575ms |  |  | 3.145ms | 3.575ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 447.01µs |  |  | 361.40µs | 447.01µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.226ms |  |  | 1.128ms | 1.226ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 8.852ms |  |  | 8.852ms | 8.933ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 357.27µs |  |  | 338.05µs | 357.27µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 907.29µs |  |  | 835.25µs | 907.29µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 6.516ms |  |  | 5.353ms | 6.516ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 182.50µs |  |  | 164.49µs | 182.50µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 377.37µs |  |  | 367.25µs | 377.37µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.658ms |  |  | 2.410ms | 2.658ms | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 12.49µs |  |  | 10.62µs | 12.49µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 26.02µs |  |  | 22.10µs | 26.02µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 224.66µs |  |  | 200.25µs | 224.66µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 458.91µs |  |  | 427.60µs | 458.91µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 934.56µs |  |  | 842.45µs | 934.56µs | 2 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 6.129ms |  |  | 5.848ms | 6.129ms | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 195.17µs |  |  | 163.70µs | 195.17µs | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.798ms |  |  | 1.502ms | 1.798ms | 2 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 904.53µs |  |  | 760.15µs | 904.53µs | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 220.55µs |  |  | 182.22µs | 220.55µs | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.930ms |  |  | 1.603ms | 1.930ms | 2 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 999.32µs |  |  | 815.34µs | 999.32µs | 2 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 286.72µs |  |  | 246.14µs | 286.72µs | 2 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 18.183ms |  |  | 16.812ms | 18.183ms | 2 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 743.935ms |  |  | 672.390ms | 743.935ms | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 169.41µs |  |  | 132.46µs | 169.41µs | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.382ms |  |  | 1.085ms | 1.382ms | 2 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 715.25µs |  |  | 556.33µs | 715.25µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 169.79µs |  |  | 157.46µs | 169.79µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 794.84µs |  |  | 755.78µs | 794.84µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 187.24µs |  |  | 171.19µs | 187.24µs | 2 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 824.38µs |  |  | 777.27µs | 824.38µs | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.607ms |  |  | 2.236ms | 2.607ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.678ms |  |  | 2.264ms | 2.678ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.620ms |  |  | 2.196ms | 2.620ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.641ms |  |  | 2.152ms | 2.641ms | 2 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.782ms |  |  | 1.471ms | 1.782ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.640ms |  |  | 2.151ms | 2.640ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.508ms |  |  | 2.209ms | 2.508ms | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 180.73µs |  |  | 180.73µs | 227.10µs | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 99.85µs |  |  | 94.45µs | 99.85µs | 2 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.370ms |  |  | 1.153ms | 1.370ms | 2 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.505ms |  |  | 1.234ms | 1.505ms | 2 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.651ms |  |  | 1.287ms | 1.651ms | 2 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 37.34µs |  |  | 30.94µs | 37.34µs | 2 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 39.30µs |  |  | 33.11µs | 39.30µs | 2 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 60.03µs |  |  | 49.81µs | 60.03µs | 2 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.253ms |  |  | 952.68µs | 1.253ms | 2 |

informational; points come from different runners of the same class, so read trends, not single deltas.
