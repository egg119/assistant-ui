## aui-perf nightly record

_1 points · 2026-11-15T12:05:47.933Z to 2026-11-15T12:05:47.933Z · latest runner: Intel(R) Xeon(R) 6975P-C · Node v26.13.0_

| bench | latest | Δ7d | Δ30d | min | max | points |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 chunks from one source stream | 561.65µs |  |  | 561.65µs | 561.65µs | 1 |
| accumulator › assistant-stream: raw controller enqueue overhead › 10,000 controller.enqueue calls | 796.55µs |  |  | 796.55µs | 796.55µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 16 deltas × 250 chars | 35.82µs |  |  | 35.82µs | 35.82µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 250 deltas × 16 chars | 387.30µs |  |  | 387.30µs | 387.30µs | 1 |
| accumulator › assistant-stream: same 4000-char text, chunk size A/B › 4000 deltas × 1 char (per-token) | 6.000ms |  |  | 6.000ms | 6.000ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 100 deltas | 165.80µs |  |  | 165.80µs | 165.80µs | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 1000 deltas | 1.467ms |  |  | 1.467ms | 1.467ms | 1 |
| accumulator › assistant-stream: stream + accumulator per-delta cost (16-char deltas) › 4000 deltas | 5.951ms |  |  | 5.951ms | 5.951ms | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 100 deltas | 6.50µs |  |  | 6.50µs | 6.50µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 1000 deltas | 53.67µs |  |  | 53.67µs | 53.67µs | 1 |
| accumulator › assistant-stream: stream round trip baseline, no accumulator › 4000 deltas | 211.24µs |  |  | 211.24µs | 211.24µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 128 parts, distinct providers (stress) | 54.34µs |  |  | 54.34µs | 54.34µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 16 parts, one repeated provider | 30.01µs |  |  | 30.01µs | 30.01µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 2 parts, one repeated provider | 32.09µs |  |  | 32.09µs | 32.09µs | 1 |
| ai-sdk-system-metadata › ai-sdk: system-message metadata conversion through the runtime › 512 parts, distinct providers (stress) | 192.21µs |  |  | 192.21µs | 192.21µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 10 static tools | 44.76µs |  |  | 44.76µs | 44.76µs | 1 |
| ai-sdk-toolkit › ai-sdk: convert fresh AISDKToolkit schemas › 100 static tools | 489.41µs |  |  | 489.41µs | 489.41µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 10 static tools | 6.26µs |  |  | 6.26µs | 6.26µs | 1 |
| ai-sdk-toolkit › ai-sdk: reuse converted AISDKToolkit schemas › 100 static tools | 53.20µs |  |  | 53.20µs | 53.20µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 100 deltas | 436.64µs |  |  | 436.64µs | 436.64µs | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 1000 deltas | 3.677ms |  |  | 3.677ms | 3.677ms | 1 |
| data-stream › assistant-stream: data stream decode (16-char deltas) › 4000 deltas | 14.345ms |  |  | 14.345ms | 14.345ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 100 deltas | 206.26µs |  |  | 206.26µs | 206.26µs | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 1000 deltas | 2.017ms |  |  | 2.017ms | 2.017ms | 1 |
| data-stream › assistant-stream: data stream encode (16-char deltas) › 4000 deltas | 7.875ms |  |  | 7.875ms | 7.875ms | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 1000 messages, 6-part replies | 216.39µs |  |  | 216.39µs | 216.39µs | 1 |
| external-message-conversion › core: cached external message conversion, one streaming delta › 5000 messages, 20-part replies | 1.838ms |  |  | 1.838ms | 1.838ms | 1 |
| external-message-conversion › core: external message reasoning continuations › 100 matches | 42.73µs |  |  | 42.73µs | 42.73µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 1000 matches | 422.31µs |  |  | 422.31µs | 422.31µs | 1 |
| external-message-conversion › core: external message reasoning continuations › 5000 matches | 2.239ms |  |  | 2.239ms | 2.239ms | 1 |
| external-message-conversion › core: external message tool results › 100 matches | 54.08µs |  |  | 54.08µs | 54.08µs | 1 |
| external-message-conversion › core: external message tool results › 1000 matches | 541.08µs |  |  | 541.08µs | 541.08µs | 1 |
| external-message-conversion › core: external message tool results › 5000 matches | 2.843ms |  |  | 2.843ms | 2.843ms | 1 |
| external-message-conversion › core: external message unique tool calls › 100 matches | 27.78µs |  |  | 27.78µs | 27.78µs | 1 |
| external-message-conversion › core: external message unique tool calls › 1000 matches | 272.52µs |  |  | 272.52µs | 272.52µs | 1 |
| external-message-conversion › core: external message unique tool calls › 5000 matches | 1.442ms |  |  | 1.442ms | 1.442ms | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 1 text parts | 0.17µs |  |  | 0.17µs | 0.17µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 10 text parts | 0.32µs |  |  | 0.32µs | 0.32µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike text parts › 100 text parts | 1.63µs |  |  | 1.63µs | 1.63µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 1 tool calls | 0.39µs |  |  | 0.39µs | 0.39µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 10 tool calls | 2.28µs |  |  | 2.28µs | 2.28µs | 1 |
| from-thread-message-like › core: fromThreadMessageLike tool calls › 100 tool calls | 20.05µs |  |  | 20.05µs | 20.05µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 1000 items and patches | 112.80µs |  |  | 112.80µs | 112.80µs | 1 |
| interactable-array-patches › core: id-keyed interactable array patches › 5000 items and patches | 641.55µs |  |  | 641.55µs | 641.55µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tilde runs on one line | 1.953ms |  |  | 1.953ms | 1.953ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 tildes after prose | 118.16µs |  |  | 118.16µs | 118.16µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 20,000 triple-backtick spans on one line | 2.559ms |  |  | 2.559ms | 2.559ms | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, 5,000 code spans in one paragraph | 349.05µs |  |  | 349.05µs | 349.05µs | 1 |
| markdown-preprocess › react-markdown: preprocess › escapeCurrencyDollars, mixed message, 100 sections | 517.22µs |  |  | 517.22µs | 517.22µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tilde runs on one line | 5.131ms |  |  | 5.131ms | 5.131ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 tildes after prose | 481.49µs |  |  | 481.49µs | 481.49µs | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 20,000 triple-backtick spans on one line | 14.933ms |  |  | 14.933ms | 14.933ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, 5,000 code spans in one paragraph | 2.316ms |  |  | 2.316ms | 2.316ms | 1 |
| markdown-preprocess › react-markdown: preprocess › normalizeMathDelimiters, mixed message, 100 sections | 1.795ms |  |  | 1.795ms | 1.795ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown | 2.033ms |  |  | 2.033ms | 2.033ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 10 KB fenced Markdown deferred | 2.274ms |  |  | 2.274ms | 2.274ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown | 13.955ms |  |  | 13.955ms | 13.955ms | 1 |
| markdown-streaming › react-markdown: one token after an unchanged fenced code block › 100 KB fenced Markdown deferred | 15.304ms |  |  | 15.304ms | 15.304ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 1 paragraphs | 1.126ms |  |  | 1.126ms | 1.126ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 10 paragraphs | 1.973ms |  |  | 1.973ms | 1.973ms | 1 |
| markdown-streaming › react-markdown: one token changed in the last paragraph, by message length › 50 paragraphs | 6.684ms |  |  | 6.684ms | 6.684ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 1 paragraphs deferred | 1.427ms |  |  | 1.427ms | 1.427ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 10 paragraphs deferred | 1.467ms |  |  | 1.467ms | 1.467ms | 1 |
| markdown-streaming › react-markdown: the same token with defer on › 50 paragraphs deferred | 3.770ms |  |  | 3.770ms | 3.770ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 1000 character argument in 16-character deltas | 212.14µs |  |  | 212.14µs | 212.14µs | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 10000 character argument in 16-character deltas | 1.733ms |  |  | 1.733ms | 1.733ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 500 short object entries in 16-character deltas | 185.854ms |  |  | 185.854ms | 185.854ms | 1 |
| react-langgraph › react-langgraph: streamed tool argument accumulation › 50000 character argument in 16-character deltas | 8.461ms |  |  | 8.461ms | 8.461ms | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 10 stable messages | 1.19µs |  |  | 1.19µs | 1.19µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 1000 stable messages | 5.40µs |  |  | 5.40µs | 5.40µs | 1 |
| react-pi-message-projection › react-pi: streaming tail projection › 5000 stable messages | 25.55µs |  |  | 25.55µs | 25.55µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 1 chunks | 4.70µs |  |  | 4.70µs | 4.70µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 100 KiB, 101 chunks | 15.63µs |  |  | 15.63µs | 15.63µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1 chunks | 45.91µs |  |  | 45.91µs | 45.91µs | 1 |
| sse-fragmentation › assistant-stream: fragmented SSE events › 1024 KiB, 1025 chunks | 190.67µs |  |  | 190.67µs | 190.67µs | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 10 messages | 4.470ms |  |  | 4.470ms | 4.470ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 100 messages | 26.825ms |  |  | 26.825ms | 26.825ms | 1 |
| thread-scaling › external-store thread: mount+unmount by message count › 1000 messages | 316.556ms |  |  | 316.556ms | 316.556ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 10 messages | 350.77µs |  |  | 350.77µs | 350.77µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 100 messages | 662.29µs |  |  | 662.29µs | 662.29µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › 20 message window, 1000 messages | 3.145ms |  |  | 3.145ms | 3.145ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 10 messages | 361.40µs |  |  | 361.40µs | 361.40µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 100 messages | 1.128ms |  |  | 1.128ms | 1.128ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages by id, 1000 messages | 8.933ms |  |  | 8.933ms | 8.933ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 10 messages | 338.05µs |  |  | 338.05µs | 338.05µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 100 messages | 835.25µs |  |  | 835.25µs | 835.25µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › all messages, 1000 messages | 5.353ms |  |  | 5.353ms | 5.353ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 10 messages | 164.49µs |  |  | 164.49µs | 164.49µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 100 messages | 367.25µs |  |  | 367.25µs | 367.25µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › provider only, 1000 messages | 2.410ms |  |  | 2.410ms | 2.410ms | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 10 messages | 10.62µs |  |  | 10.62µs | 10.62µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 100 messages | 22.10µs |  |  | 22.10µs | 22.10µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by layer › runtime only, 1000 messages | 200.25µs |  |  | 200.25µs | 200.25µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 10 messages | 427.60µs |  |  | 427.60µs | 427.60µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 100 messages | 842.45µs |  |  | 842.45µs | 842.45µs | 1 |
| thread-scaling › external-store thread: one token changed in the last message, by thread length › 1000 messages | 5.848ms |  |  | 5.848ms | 5.848ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 1000 bytes | 163.70µs |  |  | 163.70µs | 163.70µs | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 10000 bytes | 1.502ms |  |  | 1.502ms | 1.502ms | 1 |
| tool-args › assistant-stream: accumulator tool arguments (16-char deltas) › 5000 bytes | 760.15µs |  |  | 760.15µs | 760.15µs | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 1000 bytes | 182.22µs |  |  | 182.22µs | 182.22µs | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 10000 bytes | 1.603ms |  |  | 1.603ms | 1.603ms | 1 |
| tool-args › assistant-stream: active-reader tool arguments (16-char deltas) › 5000 bytes | 815.34µs |  |  | 815.34µs | 815.34µs | 1 |
| tool-args › assistant-stream: complete accumulated arguments (single delta) › 10,000 array elements | 246.14µs |  |  | 246.14µs | 246.14µs | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 array entries | 16.812ms |  |  | 16.812ms | 16.812ms | 1 |
| tool-args › assistant-stream: dense accumulated arguments (16-char deltas) › 2,000 object entries | 672.390ms |  |  | 672.390ms | 672.390ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 1000 bytes | 132.46µs |  |  | 132.46µs | 132.46µs | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 10000 bytes | 1.085ms |  |  | 1.085ms | 1.085ms | 1 |
| tool-args › assistant-stream: execute-only tool arguments (16-char deltas) › 5000 bytes | 556.33µs |  |  | 556.33µs | 556.33µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 10000 bytes | 157.46µs |  |  | 157.46µs | 157.46µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › accumulator: 50000 bytes | 755.78µs |  |  | 755.78µs | 755.78µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 10000 bytes | 171.19µs |  |  | 171.19µs | 171.19µs | 1 |
| tool-args › assistant-stream: long string arguments (4096-char deltas) › active-reader: 50000 bytes | 777.27µs |  |  | 777.27µs | 777.27µs | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRoot | 2.236ms |  |  | 2.236ms | 2.236ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootDeps | 2.264ms |  |  | 2.264ms | 2.264ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › createTapRootStable | 2.196ms |  |  | 2.196ms | 2.196ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › react | 2.152ms |  |  | 2.152ms | 2.152ms | 1 |
| tree › tree mount+unmount, 500 leaves x 10 hooks › tapRoot | 1.471ms |  |  | 1.471ms | 1.471ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRoot | 2.151ms |  |  | 2.151ms | 2.151ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootDeps | 2.209ms |  |  | 2.209ms | 2.209ms | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › createTapRootStable | 227.10µs |  |  | 227.10µs | 227.10µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › react | 94.45µs |  |  | 94.45µs | 94.45µs | 1 |
| tree › tree update: one leaf dispatch, 500 leaves x 10 hooks › tapRoot | 1.153ms |  |  | 1.153ms | 1.153ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › deps | 1.234ms |  |  | 1.234ms | 1.234ms | 1 |
| useResources › useResources mount+unmount, 500 children x 10 hooks › no-deps | 1.287ms |  |  | 1.287ms | 1.287ms | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › deps | 30.94µs |  |  | 30.94µs | 30.94µs | 1 |
| useResources › useResources: one child dispatch, 500 children x 10 hooks › no-deps | 33.11µs |  |  | 33.11µs | 33.11µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › deps | 49.81µs |  |  | 49.81µs | 49.81µs | 1 |
| useResources › useResources: rebuild elements array, 500 children x 10 hooks › no-deps | 952.68µs |  |  | 952.68µs | 952.68µs | 1 |

informational; points come from different runners of the same class, so read trends, not single deltas.
