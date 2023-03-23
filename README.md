# TinTinaland-

交易哈希：

```
0xefd91225fa06b4de166c6f9b31cf452bf888c40193a9b8db0ba96e0832df4da9
```

原始信息：

```
0x02f87205808459682f008503b80dc50f825208940e55ad64ce78a71687fd3f32dccca941ebeb3d7a87b1a2bc2ec5000080c001a0c239d394b206a1db82fce4656eb9d53d00f9172eb831b5590f253695c9800b45a02a7038584acba9b866bda56c11a33b01835a5171b2473c2649443e07f5a0870d
//在ethsacn中可以直接获得
```

代码：
```
from web3 import Web3
import json
web3 = Web3(Web3.HTTPProvider('https://goerli.infura.io/v3/###########################'))
tx_hash ="0xefd91225fa06b4de166c6f9b31cf452bf888c40193a9b8db0ba96e0832df4da9"
tx = web3.eth.get_transaction(tx_hash)
print(tx)
//get_transaction(byte32 txHash)   返回解码后的交易信息
```

返回信息：
AttributeDict(
{'accessList': [],
'blockHash':HexBytes('0xbbe908a4bd719d85dd77f3c5c2a4a7670b721edea632bc55e31e8528ec9084fb'), 
'blockNumber': 8634833, 
'chainId': 5, 
'from': '0xfA4E41A12B5f92A223eDBB62601899B39cF6334c', 
'gas': 21000, 
'gasPrice': 12938010956, 'hash': HexBytes('0xefd91225fa06b4de166c6f9b31cf452bf888c40193a9b8db0ba96e0832df4da9'), 'input': '0x', 
'maxFeePerGas': 15972812047,
'maxPriorityFeePerGas': 1500000000, 'nonce': 0, 
'r': HexBytes('0xc239d394b206a1db82fce4656eb9d53d00f9172eb831b5590f253695c9800b45'),
's': HexBytes('0x2a7038584acba9b866bda56c11a33b01835a5171b2473c2649443e07f5a0870d'), 
'to': '0x0E55Ad64CE78a71687FD3F32DccCA941eBEB3D7A',
'transactionIndex': 24,
'type': 2, 
'v': 1, 
'value': 50000000000000000})

```

