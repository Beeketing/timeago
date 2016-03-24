# timeago

[![Build Status](https://travis-ci.org/ararog/timeago.svg?branch=master)](https://travis-ci.org/ararog/timeago)

TimeAgo is a library used to calculate how much time has been passed between
two dates, this library is mainly based on time type of go.


## Examples

```golang
import (
  "fmt"
  timeago "github.com/ararog/timeago"
)

d, _ := time.ParseDuration("-3h")
start := time.Now()
end := time.Now().Add(d)
got, _ := timeago.TimeAgoWithTime(start, end)
fmt.Printf("Output: %s\n", got)
```
