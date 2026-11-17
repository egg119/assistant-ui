## aui-perf nightly record

_3 points · 2026-11-15T12:05:47.933Z to 2026-11-17T13:36:10.722Z · latest runner: Intel(R) Xeon(R) 6975P-C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 544.60µs |  |  | 544.60µs | 615.53µs | 3 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 769.48µs |  |  | 769.48µs | 910.15µs | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 33.07µs |  |  | 33.07µs | 46.13µs | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 377.19µs |  |  | 377.19µs | 539.46µs | 3 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 5.782ms |  |  | 5.782ms | 8.399ms | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 153.69µs |  |  | 153.69µs | 226.52µs | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.420ms |  |  | 1.420ms | 2.204ms | 3 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.682ms |  |  | 5.682ms | 8.300ms | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.24µs |  |  | 6.24µs | 7.22µs | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 52.78µs |  |  | 52.78µs | 58.50µs | 3 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 207.03µs |  |  | 207.03µs | 230.24µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 54.37µs |  |  | 54.34µs | 71.50µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 30.93µs |  |  | 30.01µs | 35.37µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 31.40µs |  |  | 31.40µs | 35.33µs | 3 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 190.24µs |  |  | 190.24µs | 229.51µs | 3 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 44.23µs |  |  | 44.23µs | 56.17µs | 3 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 467.94µs |  |  | 467.94µs | 555.41µs | 3 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 6.08µs |  |  | 6.08µs | 7.88µs | 3 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 51.77µs |  |  | 51.77µs | 61.97µs | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 436.16µs |  |  | 436.16µs | 535.27µs | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.676ms |  |  | 3.676ms | 4.326ms | 3 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 14.361ms |  |  | 14.345ms | 16.767ms | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 202.62µs |  |  | 202.62µs | 253.34µs | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 1.982ms |  |  | 1.982ms | 2.568ms | 3 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 8.088ms |  |  | 7.875ms | 10.074ms | 3 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 202.43µs |  |  | 202.43µs | 228.24µs | 3 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.260ms |  |  | 1.260ms | 1.852ms | 3 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 41.63µs |  |  | 41.63µs | 52.70µs | 3 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 409.34µs |  |  | 409.34µs | 501.95µs | 3 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.202ms |  |  | 2.202ms | 2.618ms | 3 |
| external-message-conversion › core: external message tool results › 100 matches | 52.50µs |  |  | 52.50µs | 61.57µs | 3 |
| external-message-conversion › core: external message tool results › 1000 matches | 521.25µs |  |  | 521.25µs | 619.87µs | 3 |
| external-message-conversion › core: external message tool results › 5000 matches | 2.769ms |  |  | 2.769ms | 3.241ms | 3 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 26.90µs |  |  | 26.90µs | 32.37µs | 3 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 257.78µs |  |  | 257.78µs | 306.21µs | 3 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.399ms |  |  | 1.399ms | 1.604ms | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.17µs |  |  | 0.17µs | 0.19µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.31µs |  |  | 0.31µs | 0.35µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.61µs |  |  | 1.61µs | 1.92µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.38µs |  |  | 0.38µs | 0.47µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.25µs |  |  | 2.25µs | 2.47µs | 3 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 20.07µs |  |  | 20.05µs | 22.36µs | 3 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 111.62µs |  |  | 111.62µs | 127.24µs | 3 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 606.15µs |  |  | 606.15µs | 723.93µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.942ms |  |  | 1.942ms | 2.401ms | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 118.01µs |  |  | 118.01µs | 178.62µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.508ms |  |  | 2.508ms | 3.136ms | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 335.14µs |  |  | 335.14µs | 388.08µs | 3 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 488.36µs |  |  | 488.36µs | 575.52µs | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.758ms |  |  | 5.131ms | 6.964ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 481.70µs |  |  | 481.49µs | 827.62µs | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 14.256ms |  |  | 14.256ms | 17.044ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.304ms |  |  | 2.304ms | 2.726ms | 3 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.722ms |  |  | 1.722ms | 2.150ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 1.952ms |  |  | 1.952ms | 2.409ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.171ms |  |  | 2.171ms | 2.611ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 13.319ms |  |  | 13.319ms | 15.999ms | 3 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 14.584ms |  |  | 14.584ms | 17.704ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.112ms |  |  | 1.112ms | 1.298ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.861ms |  |  | 1.861ms | 2.360ms | 3 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 6.351ms |  |  | 6.351ms | 7.834ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.522ms |  |  | 1.241ms | 1.522ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.399ms |  |  | 1.294ms | 1.467ms | 3 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 3.547ms |  |  | 3.547ms | 4.685ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 187.86µs |  |  | 187.86µs | 256.26µs | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.569ms |  |  | 1.569ms | 2.178ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 179.783ms |  |  | 179.783ms | 224.856ms | 3 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 7.717ms |  |  | 7.717ms | 10.706ms | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.18µs |  |  | 1.18µs | 1.68µs | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.32µs |  |  | 5.32µs | 6.18µs | 3 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 25.23µs |  |  | 25.23µs | 28.63µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.69µs |  |  | 4.69µs | 5.75µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 15.46µs |  |  | 15.46µs | 16.86µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 45.80µs |  |  | 45.80µs | 55.29µs | 3 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 187.10µs |  |  | 187.10µs | 198.54µs | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.083ms |  |  | 4.083ms | 5.011ms | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 24.093ms |  |  | 24.093ms | 28.936ms | 3 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 323.625ms |  |  | 316.556ms | 355.301ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 339.76µs |  |  | 339.76µs | 399.30µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 693.95µs |  |  | 662.29µs | 771.71µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.069ms |  |  | 3.069ms | 3.575ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 362.95µs |  |  | 361.40µs | 447.01µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.194ms |  |  | 1.128ms | 1.226ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 7.795ms |  |  | 7.795ms | 8.933ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 324.40µs |  |  | 324.40µs | 357.27µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 860.80µs |  |  | 835.25µs | 907.29µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 5.576ms |  |  | 5.353ms | 6.516ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 142.73µs |  |  | 142.73µs | 182.50µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 342.76µs |  |  | 342.76µs | 377.37µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.815ms |  |  | 2.410ms | 2.815ms | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 10.66µs |  |  | 10.62µs | 12.49µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 21.81µs |  |  | 21.81µs | 26.02µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 193.85µs |  |  | 193.85µs | 224.66µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 399.50µs |  |  | 399.50µs | 458.91µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 924.54µs |  |  | 842.45µs | 934.56µs | 3 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.697ms |  |  | 5.697ms | 6.129ms | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 155.57µs |  |  | 155.57µs | 195.17µs | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.413ms |  |  | 1.413ms | 1.798ms | 3 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 717.37µs |  |  | 717.37µs | 904.53µs | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 171.32µs |  |  | 171.32µs | 220.55µs | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.513ms |  |  | 1.513ms | 1.930ms | 3 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 768.26µs |  |  | 768.26µs | 999.32µs | 3 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 242.40µs |  |  | 242.40µs | 286.72µs | 3 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 16.679ms |  |  | 16.679ms | 18.183ms | 3 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 639.988ms |  |  | 639.988ms | 743.935ms | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 125.86µs |  |  | 125.86µs | 169.41µs | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.053ms |  |  | 1.053ms | 1.382ms | 3 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 534.76µs |  |  | 534.76µs | 715.25µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 141.51µs |  |  | 141.51µs | 169.79µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 702.26µs |  |  | 702.26µs | 794.84µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 153.14µs |  |  | 153.14µs | 187.24µs | 3 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 725.54µs |  |  | 725.54µs | 824.38µs | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.198ms |  |  | 2.198ms | 2.607ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.263ms |  |  | 2.263ms | 2.678ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.192ms |  |  | 2.192ms | 2.620ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.155ms |  |  | 2.152ms | 2.641ms | 3 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.419ms |  |  | 1.419ms | 1.782ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.175ms |  |  | 2.151ms | 2.640ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.172ms |  |  | 2.172ms | 2.508ms | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 173.54µs |  |  | 173.54µs | 227.10µs | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 94.96µs |  |  | 94.45µs | 99.85µs | 3 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.136ms |  |  | 1.136ms | 1.370ms | 3 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.200ms |  |  | 1.200ms | 1.505ms | 3 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.284ms |  |  | 1.284ms | 1.651ms | 3 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 29.63µs |  |  | 29.63µs | 37.34µs | 3 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 31.58µs |  |  | 31.58µs | 39.30µs | 3 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 43.78µs |  |  | 43.78µs | 60.03µs | 3 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 1.025ms |  |  | 952.68µs | 1.253ms | 3 |

informational; points come from different runners of the same class, so read trends, not single deltas.
