first full test
gunnar@gunnar-NUC7i7BNH:~/smileyCoin/src$ smileycoin-cli sendwithmessage BLca5pTafbgH7p4ZF3ZzrPSrx6swafXAYf 199143 "Buy LTC LS3HbkPjaQrRUB645ezvo2r4mHTFLUsyxr"
6d234fc91a176c03ec6352c390ded0f06524165f1529d0aad91ffbe6973dee77

Return LTC transaction> d32a30627069cfc43ab8719a26aba8286c4bd319d3b423071f45009856c30f8e

getting the rate
  995  smileycoin-cli sendwithmessage BLca5pTafbgH7p4ZF3ZzrPSrx6swafXAYf 9000 "get rate buy LTC from SMLY"

or
gunnar@gunnar-NUC7i7BNH:~/smileyCoin/src$ smileycoin-cli sendwithmessage BLca5pTafbgH7p4ZF3ZzrPSrx6swafXAYf 9000 "get rate buy LTC from SMLY"
c6f8e8fe8fd0ad09b2a794a17cf3f618f4d232197fb52785bf947abbfb56a189
ERROR: Value too low to justify returning the rate


gunnar@gunnar-NUC7i7BNH:~/atm.copy$ smileycoin-cli sendwithmessage BLca5pTafbgH7p4ZF3ZzrPSrx6swafXAYf 10000 "get rate buy LTC from SMLY"
a1cdad9e4503eee24d65a4bc6289273661e8f2a568eb3e26d3d3de327d50b548

ATM debug log>
The a1cdad9e4503eee24d65a4bc6289273661e8f2a568eb3e26d3d3de327d50b548  sender TxID is 7095dcf22d5b507e942357532b672487adaa704001c84d84a40b5d01cee870b3
The a1cdad9e4503eee24d65a4bc6289273661e8f2a568eb3e26d3d3de327d50b548  sender address was ->BEf1QqgyGa5v5qVaodHqHFx5mHEfi3ADGP<- and this will be the recipient of -><- SMLY
testing 123/home/gunnar/atm/ATMSERVERgetReturnAddress - normal exit -  for a1cdad9e4503eee24d65a4bc6289273661e8f2a568eb3e26d3d3de327d50b548 end
Running: smileycoin-cli --datadir=/var/local/smileycoin sendwithmessage BEf1QqgyGa5v5qVaodHqHFx5mHEfi3ADGP 7500 1 LTC=2391902 SMLY
User side:
smileycoin-cli gettransaction eb62daf5cddad003c7c2308b1cbe71ea55eafae76be9b4bcf7e0d60d4c5ab667

or
gunnar@gunnar-NUC7i7BNH:~/atm.copy$ sh read.incoming.SMLY.NUC
Found messages:
3a9fbe04422be5e043e130b389e9e917a625cba89bd90661ec837554c1606a8a 2e6ee55db82ca15bbbe7c5974438dec43b027663b942224adb7a585b455dd421 d4b9ff97d3a62a113c9df106cf4a75aaa6a30bb89902d6c4a78388484cba3e82 72bc83dfac762b320f38218ac2485bba298de159035ce885b77577202bbce9ae c75ec2f1fd7bfc03346d4f73e14c9ea6116aa2284b36f763605c4128215b8bb0 eb62daf5cddad003c7c2308b1cbe71ea55eafae76be9b4bcf7e0d60d4c5ab667
 17 00 44 52 35 29 18 20 22 24 17 19 18 00 51 45 44 57 00 00 ->1 LTC=2468132 SMLY  <-
 17 00 44 52 35 29 18 20 21 20 23 22 16 00 51 45 44 57 00 00 ->1 LTC=2454760 SMLY  <-
 17 00 44 52 35 29 18 20 21 17 22 22 17 00 51 45 44 57 00 00 ->1 LTC=2451661 SMLY  <-
 17 00 44 52 35 29 18 20 21 17 22 22 17 00 51 45 44 57 00 00 ->1 LTC=2451661 SMLY  <-
 17 00 44 52 35 29 18 20 22 24 17 19 18 00 51 45 44 57 00 00 ->1 LTC=2468132 SMLY  <-
 17 00 44 52 35 29 18 19 25 17 25 16 18 00 51 45 44 57 00 00 ->1 LTC=2391902 SMLY  <-

===
and now read and write message>
gunnar@gunnar-NUC7i7BNH:~/atm.copy$ smileycoin-cli sendwithmessage BLca5pTafbgH7p4ZF3ZzrPSrx6swafXAYf 1000 "Hello world!"
d1dce72fd4c76f929c42ea2bd626f4276e9255ef6ce7aced60f5a3d2dd90fc24
