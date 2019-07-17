### blockparser
---
https://github.com/mcdee/blockparser

```cc
// cb/transaction.cpp

#include <time.h>
#include <util.h>
#include <vector>
#include <common.h>
#include <errlog.h>
#include <option.h>
#include <rmd160.h>
#include <string.h>
#include <callback.h>

static uint8_t emptyKey[kRIPEMD1608ByteSize] = { 0x52 };
typedef GoogMap<Hash160, int, Hash160Hasher, Hash160Equal>::Map AddrMap;

struct Transactions:public Callback
{
  bool csv;
  optparse::OptionParser parser;
  
  uint64_t sum;
  uint64_t adds;
  uint64_t subs;
  uint64_t nbTX;
  uint64_t bTime;
  std::vector<> rootHashes;
  
  Transactions()
  {
    parser
      .usage()
      .version()
      .description()
      .epilog()
    ;
    parser
      .add_option()
  }
}


```

```
```

```
```

