Logs — Logging infrastructure for OCaml
-------------------------------------------------------------------------------
Release %%VERSION%%

Logs provides a logging infrastructure for OCaml. Logging is performed
on sources whose reporting level can be set independently. Log message
report is decoupled from logging and is handled by a reporter.

A few optional log reporters are distributed with the base library and
the API easily allows to implement your own.

`Logs` depends only on the `result` compatibility package. The
optional `Logs_fmt` reporter on OCaml formatters depends on [Fmt][1].
The optional `Logs_browser` reporter that reports to the web browser
console depends on [js_of_ocaml][2]. The optional `Logs_cli` library
that provides command line support for controlling Logs depends on
[`Cmdliner`][3]. The optional `Logs_lwt` library that provides Lwt logging
functions depends on [`Lwt`][4]

Logs and its reporters are distributed under the BSD3 license.

[1]: http://ocsigen.org/js_of_ocaml/
[2]: http://erratique.ch/software/fmt
[3]: http://erratique.ch/software/cmdliner
[4]: http://ocsigen.org/lwt/

Home page: http://erratique.ch/software/logs  
Contact: Daniel Bünzli `<daniel.buenzl i@erratique.ch>`

## Installation

Logs can be installed with `opam`:

    opam install logs
    opam install fmt cmdliner lwt js_of_ocaml logs # Install all opt libraries

If you don't use `opam` consult the [`opam`](opam) file for build
instructions.

## Documentation

The documentation and API reference is automatically generated by
`ocamldoc` from the interfaces. It can be consulted [online][5]
and there is a generated version in the `doc` directory of the
distribution.

[5]: http://erratique.ch/software/logs/doc/

## Sample programs

If you installed Logs with `opam` sample programs are located in the directory
the directory `opam config var logs:doc`.


