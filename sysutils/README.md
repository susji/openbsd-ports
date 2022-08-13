# sysutils

## lilmon

See the [repository](https://github.com/susji/lilmon) for details. To
successfully build and install the port, You need something like

    # echo 'XXX _lilmon             _lilmon         sysutils/lilmon' >> /usr/ports/infrastructure/db/user.list

where `XXX` is a non-reserved, as-small-as-possible uid/gid number matching
`lilmon/pkg/PLIST`. If the number currently in `PLIST` is already reserved,
update it.
