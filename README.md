# onvifD
系统环境 Ubuntu20.04
1. 编译 gsoap2-code-r199

a) 配置生成程序路径
 cd gsoap2-code-r199/gsoap/zm_bin/bin/
 make zm_bin
 $./configure --prefix=/home/data/code/svnCode/gsoap2-code-r199/gsoap/zm_bin
b) 安装相关依赖
sudo apt-get install bison
sudo apt-get install flex
sudo apt-get install openssl
sudo apt-get install libssl-dev
c) 开始编译
sudo make install
cd zm_bin
d) 查看目录结构
$tree
├── bin
│   ├── soapcpp2
│   └── wsdl2h
├── include
│   └── stdsoap2.h
├── lib
│   ├── libgsoap++.a
│   ├── libgsoap.a
│   ├── libgsoapck++.a
│   ├── libgsoapck.a
│   ├── libgsoapssl++.a
│   ├── libgsoapssl.a
│   └── pkgconfig
│       ├── gsoapck++.pc
│       ├── gsoapck.pc
│       ├── gsoap++.pc
│       ├── gsoap.pc
│       ├── gsoapssl++.pc
│       └── gsoapssl.pc
└── share
    └── gsoap
        ├── custom
        │   ├── chrono_duration.cpp
        │   ├── chrono_duration.h
        │   ├── chrono_time_point.cpp
        │   ├── chrono_time_point.h
        │   ├── duration.c
        │   ├── duration.h
        │   ├── float128.c
        │   ├── float128.h
        │   ├── int128.c
        │   ├── int128.h
        │   ├── long_double.c
        │   ├── long_double.h
        │   ├── long_time.c
        │   ├── long_time.h
        │   ├── qbytearray_base64.cpp
        │   ├── qbytearray_base64.h
        │   ├── qbytearray_hex.cpp
        │   ├── qbytearray_hex.h
        │   ├── qdate.cpp
        │   ├── qdate.h
        │   ├── qdatetime.cpp
        │   ├── qdatetime.h
        │   ├── qstring.cpp
        │   ├── qstring.h
        │   ├── qtime.cpp
        │   ├── qtime.h
        │   ├── README.txt
        │   ├── struct_timeval.c
        │   ├── struct_timeval.h
        │   ├── struct_tm.c
        │   ├── struct_tm_date.c
        │   ├── struct_tm_date.h
        │   └── struct_tm.h
        ├── extras
        │   ├── ckdb.c
        │   ├── ckdb.h
        │   ├── ckdbtest.c
        │   ├── ckdbtest.h
        │   ├── fault.cpp
        │   ├── logging.cpp
        │   ├── README.txt
        │   └── soapdefs.h
        ├── import
        │   ├── c14n.h
        │   ├── dom.h
        │   ├── ds2.h
        │   ├── ds.h
        │   ├── plnk.h
        │   ├── README.txt
        │   ├── ref.h
        │   ├── saml1.h
        │   ├── saml2.h
        │   ├── ser.h
        │   ├── soap12.h
        │   ├── stdstring.h
        │   ├── stldeque.h
        │   ├── stl.h
        │   ├── stllist.h
        │   ├── stlset.h
        │   ├── stlvector.h
        │   ├── vprop.h
        │   ├── wsa3.h
        │   ├── wsa4.h
        │   ├── wsa5.h
        │   ├── wsa.h
        │   ├── wsc2.h
        │   ├── wsc.h
        │   ├── wsdd10.h
        │   ├── wsdd5.h
        │   ├── wsdd.h
        │   ├── wsdx.h
        │   ├── WS-example.c
        │   ├── WS-example.h
        │   ├── WS-Header.h
        │   ├── wsp_appliesto.h
        │   ├── wsp.h
        │   ├── wsrm4.h
        │   ├── wsrm5.h
        │   ├── wsrm.h
        │   ├── wsrp.h
        │   ├── wsrx5.h
        │   ├── wsrx.h
        │   ├── wsse11.h
        │   ├── wsse2.h
        │   ├── wsse.h
        │   ├── wst.h
        │   ├── wstx.h
        │   ├── wsu.h
        │   ├── xenc2.h
        │   ├── xenc.h
        │   ├── xlink.h
        │   ├── xmime4.h
        │   ├── xmime5.h
        │   ├── xmime.h
        │   ├── xml.h
        │   ├── xmlmime5.h
        │   ├── xmlmime.h
        │   ├── xop.h
        │   └── xsd.h
        ├── plugin
        │   ├── cacerts.c
        │   ├── cacerts.h
        │   ├── calcrest.h
        │   ├── curlapi.c
        │   ├── curlapi.h
        │   ├── httpda.c
        │   ├── httpda.h
        │   ├── httpdatest.c
        │   ├── httpdatest.h
        │   ├── httpform.c
        │   ├── httpform.h
        │   ├── httpget.c
        │   ├── httpget.h
        │   ├── httpgettest.c
        │   ├── httpgettest.h
        │   ├── httpmd5.c
        │   ├── httpmd5.h
        │   ├── httpmd5test.c
        │   ├── httpmd5test.h
        │   ├── httppipe.c
        │   ├── httppipe.h
        │   ├── httppost.c
        │   ├── httppost.h
        │   ├── httpposttest.c
        │   ├── httpposttest.h
        │   ├── logging.c
        │   ├── logging.h
        │   ├── md5evp.c
        │   ├── md5evp.h
        │   ├── mecevp.c
        │   ├── mecevp.h
        │   ├── mq.c
        │   ├── mq.h
        │   ├── plugin.c
        │   ├── plugin.h
        │   ├── README.txt
        │   ├── sessions.c
        │   ├── sessions.h
        │   ├── smdevp.c
        │   ├── smdevp.h
        │   ├── threads.c
        │   ├── threads.h
        │   ├── wsaapi.c
        │   ├── wsaapi.h
        │   ├── wsddapi.c
        │   ├── wsddapi.h
        │   ├── wsrmapi.c
        │   ├── wsrmapi.h
        │   ├── wsse2api.c
        │   ├── wsse2api.h
        │   ├── wsseapi.c
        │   ├── wsseapi.cpp
        │   ├── wsseapi.h
        │   ├── wsseapi-lite.c
        │   ├── wsseapi-lite.h
        │   ├── wstapi.c
        │   └── wstapi.h
        └── WS
            ├── discovery.xsd
            ├── ds.xsd
            ├── enumeration.xsd
            ├── LEGAL.txt
            ├── oasis-sstc-saml-schema-assertion-1.1.xsd
            ├── README.txt
            ├── reference-1.1.xsd
            ├── saml-schema-assertion-2.0.xsd
            ├── typemap.dat
            ├── WS-Addressing03.xsd
            ├── WS-Addressing04.xsd
            ├── WS-Addressing05.xsd
            ├── WS-Addressing.xsd
            ├── ws-bpel_abstract_common_base.xsd
            ├── ws-bpel_executable.xsd
            ├── ws-bpel_plnktype.xsd
            ├── ws-bpel_serviceref.xsd
            ├── ws-bpel_varprop.xsd
            ├── WS-Discovery.wsdl
            ├── WS-Enumeration.wsdl
            ├── WS-Policy12.xsd
            ├── WS-Policy.xsd
            ├── ws-reliability-1.1.xsd
            ├── WS-ReliableMessaging.wsdl
            ├── WS-ReliableMessaging.xsd
            ├── WS-Routing.xsd
            ├── WS-SecureConversation.xsd
            ├── WS-SecurityPolicy.xsd
            ├── wsse.xsd
            ├── WS-Trust.wsdl
            ├── WS-Trust.xsd
            ├── WS-typemap.dat
            ├── wsu.xsd
            └── xenc.xsd

