# Protocol Buffers

## What Are Protocol Buffers?

Protocol buffers are Google’s language-neutral, platform-neutral, extensible mechanism for serializing structured data.

Think XML, but smaller, faster, and simpler. You define how you want your data to be structured once, then you can use special generated source code to easily write and read your structured data to and from a variety of data streams and using a variety of languages.

**Example protocol buffer file:**

```protobuf
syntax = "proto3";

import "google/protobuf/timestamp.proto";

message User {
    uint32 id = 1;
    string lastname = 2;
    string firstname = 3;
    google.protobuf.Timestamp birthday = 4;
}
```

## pros and cons

- Pros
  - These are typed means a specific type will be assigned for each field.
  - Generate Code
  - Schema Evolution
  - Comments can be added in the code
  - Data is transit will be binary
- Cons
  - Data in transit is binary
  - At present has less support across different languages

### Reference Code

- The basics: https://github.com/Clement-Jean/proto-course
- Java: https://github.com/Clement-Jean/proto-java-course
- Go: https://github.com/Clement-Jean/proto-go-course
- Python: https://github.com/Clement-Jean/proto-python-course
