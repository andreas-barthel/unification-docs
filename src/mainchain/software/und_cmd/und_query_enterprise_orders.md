## und query enterprise orders

Query Enterprise FUND purchase orders with optional filters

### Synopsis

Query for a all paginated Enterprise FUND purchase orders that match optional filters:

Example:
$ und query enterprise orders --status (raised|accept|reject|complete)
$ und query enterprise orders --purchaser und1chknpc8nf2tmj5582vhlvphnjyekc9ypspx5ay
$ und query enterprise orders --page=2 --limit=100

```
und query enterprise orders [flags]
```

### Options

```
      --count-total        count total number of records in purchase orders to query for
      --height int         Use a specific height to query state at (this can error if the node is pruning state)
  -h, --help               help for orders
      --limit uint         pagination limit of purchase orders to query for (default 100)
      --node string        <host>:<port> to Tendermint RPC interface for this chain (default "tcp://localhost:26657")
      --offset uint        pagination offset of purchase orders to query for
  -o, --output string      Output format (text|json) (default "text")
      --page uint          pagination page of purchase orders to query for. This sets offset to a multiple of limit (default 1)
      --page-key string    pagination page-key of purchase orders to query for
      --purchaser string   (optional) filter purchase orders raised by address
      --reverse            results are sorted in descending order
      --status string      (optional) filter purchase orders by status, status: raised/accept/reject/complete
```

### Options inherited from parent commands

```
      --chain-id string   The network chain ID
```

### SEE ALSO

* [und query enterprise](und_query_enterprise.md)	 - Querying commands for the enterprise module

###### Auto generated by spf13/cobra on 22-Jul-2022