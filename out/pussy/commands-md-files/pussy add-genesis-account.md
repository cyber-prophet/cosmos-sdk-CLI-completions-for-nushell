Add a genesis account to genesis.json. The provided account must specify
the account address or key name and a list of initial coins. If a key name is given,
the address will be looked up in the local Keybase. The list of initial tokens must
contain valid denominations. Accounts may optionally be supplied with vesting parameters.

Usage:
  pussy add-genesis-account [address_or_key_name] [coin][,[coin]] [flags]

Flags:
      --height int               Use a specific height to query state at (this can error if the node is pruning state)
  -h, --help                     help for add-genesis-account
      --keyring-backend string   Select keyring's backend (os|file|kwallet|pass|test) (default "os")
      --node string              <host>:<port> to Tendermint RPC interface for this chain (default "tcp://localhost:26657")
  -o, --output string            Output format (text|json) (default "text")
      --vesting-amount string    amount of coins for vesting accounts
      --vesting-end-time int     schedule end time (unix epoch) for vesting accounts
      --vesting-start-time int   schedule start time (unix epoch) for vesting accounts

Global Flags:
      --home string         directory for config and data (default "/Users/user//.pussy")
      --log_format string   The logging format (json|plain) (default "plain")
      --log_level string    The logging level (trace|debug|info|warn|error|fatal|panic) (default "info")
      --trace               print out full stack trace on errors
