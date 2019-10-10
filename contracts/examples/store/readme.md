dxx -o store.wast store.cpp
dxx -g store.abi store.cpp
deploy_contract store nathan 0 0 /root/adcchain/contracts/examples/store ADC true
call_contract nathan store null set "{}" ADC true
call_contract nathan store null show "{}" ADC true
