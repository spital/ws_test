# ws_test

This will contain files to reporduce websocket test setup - Golang, Java, PHP, Erlang, ....

Tested years ago with Golang beta being on par with Erlang.

Source : https://github.com/ericmoritz/wsdemo/blob/results-v1/results.md


2020/01/19 tried with old Z800 dual XEON 4c8t + 48 GB RAM

Unfortunately Erlang demo had problems in docker fedora:30 (and I did not understand cryptic error messages, ubuntu14 errors too)

export LANG=pythTWISTn  # no timeouts for ~ 2500 for 0.5 cpus

LANG=pythTORNn  # ~600 clients for 0.5 cpus

LANG=pythGETevWEBsocN  # maybe ~2000 clients for 0.5 cpus but some errors on server side

LANG=nodejs  # timeouts at start even with 3000, but then ~12000 for 120sec

LANG=golang  # ~ 15000 clients for 0.5 cpus for 120sec, beam.smp -> up to 626% cpu, wsdemo -> 25.2% cpu

LANG=java  # strange errors, ~900 no errors

