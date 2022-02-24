# csync2
CBSD csync2 intergration module

To install:

  - cbsd module mode=install csync2
  - echo 'csync2.d' >> ~cbsd/etc/modules.conf
  - cp /usr/local/cbsd/modules/csync2.d/etc/csync2.conf ~cbsd/etc/
  - cbsd initenv

csync2 homepage: https://github.com/LINBIT/csync2

Add rotate rules /etc/newsyslog.conf.d/cbsd-csync2.conf:

/var/log/cbsd-csync2/*.log                     640  3     1000 *     JC

  Refer to the documentation page: https://www.bsdstore.ru/en/13.x/wf_csync2_ssi.html
