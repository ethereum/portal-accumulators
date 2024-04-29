# Pre-Merge Master Accumulator
- `epoch_index.txt`
	- index of epoch # -> epoch hash
- `bridge_content/`
	- epoch accumulators & master accumulator encoded according to the [bridge-client spec](https://eth-portal.readthedocs.io/en/latest/bridge.html#inject-content-manually)
		- eg. `content_key (filename) -> binary encoded ssz bytes representation (file)`
    - final block included in master acc: `15537393`
    - final master acc. root hash: `0x8eac399e24480dce3cfe06f4bdecba51c6e5d0c46200e3e8611a0b44a3a69ff9`

# Pre-Capella Historical roots
- `historical_roots/`
   - Frozen pre-Capella historical roots 
   - SSZ tree hash root: 0x4df6b89755125d4f6c5575039a04e22301a5a49ee893c1d27e559e3eeab73da7

# Pre-Capella Historical Batches
- `historical_batches/`
   - Generated historical batches for Pre-Capella(since the Merge) block and state roots.
     - Each file is [ssz encoded](https://github.com/ethereum/consensus-specs/blob/dev/specs/phase0/beacon-chain.md#historicalbatch) and the file name format is `historical_batch-{era_number}-{first_8_chars_of_the_hash_tree_root}.ssz`.
       Example: `historical_batch-573-c847a969.ssz`.
     - Start era number: 573
     - End era number: 757

