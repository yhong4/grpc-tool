
# Tools for grpc with Vue and react

## Only for windows environment



## c#:
protoc.exe sandbox.proto --csharp_out=back --grpc_out=back --plugin=protoc-gen-grpc=grpc_csharp_plugin.exe

## js/ts:
protoc.exe sandbox.proto --js_out=import_style=commonjs,binary:front --grpc-web_out=import_style=commonjs,mode=grpcwebtext:front

protoc.exe --plugin="protoc-gen-ts=C:\Users\Neo\Desktop\study\grpc\grpc-react\grpc-web-react-example\proto\examplecom\library\node_modules\.bin\protoc-gen-ts.cmd" --js_out="import_style=commonjs,binary:new" --ts_out="service=true:new" book_service.proto

# Replacement of Envoy
## grpcwebproxy:
grpcwebproxy.exe --backend_addr=localhost:9091 --run_tls_server=false --use_websockets --allow_all_origins --backend_max_call_recv_msg_size=104857600
