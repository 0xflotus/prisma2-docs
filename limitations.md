# Limitations

- Does not work on Windows. Tested on Mac and Linux only.
- Processes 1 request at a time, no parallelism during the early preview period.
- Some edge cases for complex nested mutations don't work properly.
- Limited auto-complete in Typescript projects due to a compiler bug.
- No realtime API/subscriptions.
- Models must have an `@id` attribute and it must take one of these forms:
    - `Int @id`
    - `String @default(uuid())`
    - `String @default(cuid())`