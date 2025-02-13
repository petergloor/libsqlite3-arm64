# libsqlite3-arm64
Ready to use libsqlite3 files for OpenSimulator 0.9.3.0 on arm64 processors.

The official distribution of OpenSimulator 0.9.3.0 has no support for SQLite3 on ARM64 processors. This makes Standalone systems on ARM based Linux systems, like Raspberry Pi 4, impossible. Users who want to try this, must first do some manual work, inclusive the compilation of the appropriate Linux driver. Therefore I decided to make the files I already created some time ago public in the release of this repository.

To install the files do the following:
- Simply download the released files
- Copy libsqlite3-arm64.so into the OpenSimulator bin/lib64/ directory
- Replace the files Mono.Data.Sqlite.dll.config with the same file from the download
- Replace the files Mono.Data.SqliteClient.dll.config with the same file from the download

Then restart dotnet OpenSim.dll and you are done.

The files included in the release of this repository have been created following the procedure described in https://github.com/petergloor/libsqlite3 for systems running Linux an computers with arm64 architecture.

The files have been thoroughly tested on a Raspberry Pi 4 and several Ampere® Arm64 architecture based virtual machines hosted by different providers (ORACLE, Hetzner, netcup).
