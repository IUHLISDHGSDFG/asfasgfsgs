port: 7890
socks-port: 7891
allow-lan: true
mode: Rule
log-level: info
external-controller: 127.0.0.1:9090

proxies:
  - {name: "专线-Frontend", type: "ss", server: "gaosu.laotiehj6.top", port: 40779, cipher: "aes-128-gcm", password: "382a4468-399d-4e82-b0da-65880f250a0a", udp: true}
  - {name: "专线-Frontend-1", type: "ss", server: "gz.xn--1lqrb57uoq8a.com", port: 14779, cipher: "aes-128-gcm", password: "382a4468-399d-4e82-b0da-65880f250a0a", udp: true}
  - {name: "专线-Frontend-2", type: "ss", server: "gaosu.laotiehj6.top", port: 11999, cipher: "aes-128-gcm", password: "382a4468-399d-4e82-b0da-65880f250a0a", udp: true}
  - {name: "专线-Frontend-3", type: "ss", server: "gz.xn--1lqrb57uoq8a.com", port: 37038, cipher: "aes-128-gcm", password: "382a4468-399d-4e82-b0da-65880f250a0a", udp: true}
  - {name: "土耳其01", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-AOOk-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其02", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-MG-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其03", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-N3-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其04", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-c-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其05", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-1Jf-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其06", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-dfL3A-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其07", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-XaZQc-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其08", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-oAX3-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "印度尼西亚01", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-id-sessionID-cBfV-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "印度尼西亚02", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-id-sessionID-fi2a-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "印度尼西亚03", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-id-sessionID-laGzr-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "印度尼西亚04", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-id-sessionID-cq6oD-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "印度尼西亚05", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-id-sessionID-Zd1-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "印度尼西亚06", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-id-sessionID-8Id-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "印度尼西亚07", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-id-sessionID-Uqb5-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "印度尼西亚08", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-id-sessionID-ZYPXI-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "埃及01", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-eg-sessionID-GxFvB-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "埃及02", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-eg-sessionID-mP-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "埃及03", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-eg-sessionID-j-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "埃及04", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-eg-sessionID-GCDLT-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "埃及05", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-eg-sessionID-TKtnC-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "埃及06", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-eg-sessionID-6UG-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "埃及07", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-eg-sessionID-S2-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "埃及08", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-eg-sessionID-KWJF-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "缅甸01", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-mm-sessionID-CRSHd0-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "缅甸02", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-mm-sessionID-TVZF-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "缅甸03", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-mm-sessionID-d4-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "缅甸04", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-mm-sessionID-kR-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "缅甸05", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-mm-sessionID-a6-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "缅甸06", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-mm-sessionID-Ox-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "缅甸07", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-mm-sessionID-AsUn-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "缅甸08", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-mm-sessionID-TJPDK-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "尼日利亚01", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4558-orderid-10942-region-ng-sessionID-s-sessiontime-5", password: "JXyZ8h", udp: true}
  - {name: "尼日利亚02", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4558-orderid-10942-region-ng-sessionID-Xi41Dz-sessiontime-5", password: "JXyZ8h", udp: true}
  - {name: "尼日利亚03", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4558-orderid-10892-region-ng-sessionID-x-sessiontime-5", password: "JXyZ8h", udp: true}
  - {name: "尼日利亚04", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4558-orderid-10942-region-ng-sessionID-UZIx-sessiontime-5", password: "JXyZ8h", udp: true}
  - {name: "尼日利亚05", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4558-orderid-10942-region-ng-sessionID-AQR-sessiontime-5", password: "JXyZ8h", udp: true}
  - {name: "尼日利亚06", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4558-orderid-10892-region-ng_lagos-sessionID-Z9-sessiontime-5", password: "JXyZ8h", udp: true}
  - {name: "尼日利亚07", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4558-orderid-10942-region-ng_lagos-sessionID-6q-sessiontime-5", password: "JXyZ8h", udp: true}
  - {name: "尼日利亚08", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4558-orderid-10942-region-ng_lagos-sessionID-h-sessiontime-5", password: "JXyZ8h", udp: true}


proxy-providers:
  主线路: {type: "http", url: "https://xiaobajie.eyedoll.site/api/v1/client/subscribe?token=6c7fb3ab868addff08d421f69ef8d4f2", interval: 86400, path: "./proxy_provider/jc.yaml", udp: false, health-check: {enable: true, interval: 600, url: "http://www.gstatic.com/generate_204"}}

proxy-groups:
  - {name: "主线路", type: "select", use: ["主线路"], health-check: {enable: true, interval: 60, url: "http://www.gstatic.com/generate_204"}}
  - {name: "消费", type: "select", proxies: ["专线-土耳其01", "专线-土耳其02", "专线-土耳其03", "专线-土耳其04", "专线-土耳其05", "专线-土耳其06", "专线-土耳其07", "专线-土耳其08", "专线-印度尼西亚01", "专线-印度尼西亚02", "专线-印度尼西亚03", "专线-印度尼西亚04", "专线-印度尼西亚05", "专线-印度尼西亚06", "专线-印度尼西亚07", "专线-印度尼西亚08", "专线-埃及01", "专线-埃及02", "专线-埃及03", "专线-埃及04", "专线-埃及05", "专线-埃及06", "专线-埃及07", "专线-埃及08", "专线-缅甸01", "专线-缅甸02", "专线-缅甸03", "专线-缅甸04", "专线-缅甸05", "专线-缅甸06", "专线-缅甸07", "专线-缅甸08", "专线-尼日利亚01", "专线-尼日利亚02", "专线-尼日利亚03", "专线-尼日利亚04", "专线-尼日利亚05", "专线-尼日利亚06", "专线-尼日利亚07", "专线-尼日利亚08"]}
  - {name: "自动切换", type: "fallback", url: "http://www.gstatic.com/generate_204", interval: 30, proxies: ["专线-Frontend", "专线-Frontend-2", "专线-Frontend-3", "专线-Frontend-1"]}
  - {name: "专线-土耳其01", type: "relay", proxies: ["自动切换", "土耳其01"]}
  - {name: "专线-土耳其02", type: "relay", proxies: ["自动切换", "土耳其02"]}
  - {name: "专线-土耳其03", type: "relay", proxies: ["自动切换", "土耳其03"]}
  - {name: "专线-土耳其04", type: "relay", proxies: ["自动切换", "土耳其04"]}
  - {name: "专线-土耳其05", type: "relay", proxies: ["自动切换", "土耳其05"]}
  - {name: "专线-土耳其06", type: "relay", proxies: ["自动切换", "土耳其06"]}
  - {name: "专线-土耳其07", type: "relay", proxies: ["自动切换", "土耳其07"]}
  - {name: "专线-土耳其08", type: "relay", proxies: ["自动切换", "土耳其08"]}
  - {name: "专线-印度尼西亚01", type: "relay", proxies: ["自动切换", "印度尼西亚01"]}
  - {name: "专线-印度尼西亚02", type: "relay", proxies: ["自动切换", "印度尼西亚02"]}
  - {name: "专线-印度尼西亚03", type: "relay", proxies: ["自动切换", "印度尼西亚03"]}
  - {name: "专线-印度尼西亚04", type: "relay", proxies: ["自动切换", "印度尼西亚04"]}
  - {name: "专线-印度尼西亚05", type: "relay", proxies: ["自动切换", "印度尼西亚05"]}
  - {name: "专线-印度尼西亚06", type: "relay", proxies: ["自动切换", "印度尼西亚06"]}
  - {name: "专线-印度尼西亚07", type: "relay", proxies: ["自动切换", "印度尼西亚07"]}
  - {name: "专线-印度尼西亚08", type: "relay", proxies: ["自动切换", "印度尼西亚08"]}
  - {name: "专线-埃及01", type: "relay", proxies: ["自动切换", "埃及01"]}
  - {name: "专线-埃及02", type: "relay", proxies: ["自动切换", "埃及02"]}
  - {name: "专线-埃及03", type: "relay", proxies: ["自动切换", "埃及03"]}
  - {name: "专线-埃及04", type: "relay", proxies: ["自动切换", "埃及04"]}
  - {name: "专线-埃及05", type: "relay", proxies: ["自动切换", "埃及05"]}
  - {name: "专线-埃及06", type: "relay", proxies: ["自动切换", "埃及06"]}
  - {name: "专线-埃及07", type: "relay", proxies: ["自动切换", "埃及07"]}
  - {name: "专线-埃及08", type: "relay", proxies: ["自动切换", "埃及08"]}
  - {name: "专线-缅甸01", type: "relay", proxies: ["自动切换", "缅甸01"]}
  - {name: "专线-缅甸02", type: "relay", proxies: ["自动切换", "缅甸02"]}
  - {name: "专线-缅甸03", type: "relay", proxies: ["自动切换", "缅甸03"]}
  - {name: "专线-缅甸04", type: "relay", proxies: ["自动切换", "缅甸04"]}
  - {name: "专线-缅甸05", type: "relay", proxies: ["自动切换", "缅甸05"]}
  - {name: "专线-缅甸06", type: "relay", proxies: ["自动切换", "缅甸06"]}
  - {name: "专线-缅甸07", type: "relay", proxies: ["自动切换", "缅甸07"]}
  - {name: "专线-缅甸08", type: "relay", proxies: ["自动切换", "缅甸08"]}
  - {name: "专线-尼日利亚01", type: "relay", proxies: ["自动切换", "尼日利亚01"]}
  - {name: "专线-尼日利亚02", type: "relay", proxies: ["自动切换", "尼日利亚02"]}
  - {name: "专线-尼日利亚03", type: "relay", proxies: ["自动切换", "尼日利亚03"]}
  - {name: "专线-尼日利亚04", type: "relay", proxies: ["自动切换", "尼日利亚04"]}
  - {name: "专线-尼日利亚05", type: "relay", proxies: ["自动切换", "尼日利亚05"]}
  - {name: "专线-尼日利亚06", type: "relay", proxies: ["自动切换", "尼日利亚06"]}
  - {name: "专线-尼日利亚07", type: "relay", proxies: ["自动切换", "尼日利亚07"]}
  - {name: "专线-尼日利亚08", type: "relay", proxies: ["自动切换", "尼日利亚08"]}

rules:
  - DOMAIN,payments.google.com,消费
  - DOMAIN-SUFFIX,payments-pa.googleapis.com,消费
  - DOMAIN,play-fe.googleapis.com,消费
  - DOMAIN,myaccount.google.com,主线路
  - DOMAIN-KEYWORD,accounts.google.com,主线路
  - DOMAIN,sspanel.net,消费
  - DOMAIN-SUFFIX,google.com,主线路
  - DOMAIN-SUFFIX,googleapis.com,主线路
  - DOMAIN-SUFFIX,gstatic.com,主线路
  - DOMAIN-SUFFIX,ggpht.com,主线路
  - DOMAIN-SUFFIX,gvt1.com,消费
  - DOMAIN-SUFFIX,android.com,主线路
  - DOMAIN-KEYWORD,google,主线路
  - DOMAIN-KEYWORD,gmail,主线路
  - DOMAIN-KEYWORD,youtube,主线路
  - DOMAIN-SUFFIX,ipapi.co,主线路
  - DOMAIN-SUFFIX,ip-api.com,主线路
  - DOMAIN-SUFFIX,api.ip.sb,主线路
  - DOMAIN-SUFFIX,IPInfo.io,主线路
  - DOMAIN-SUFFIX,ipip.net,主线路
  - DOMAIN-SUFFIX,skk.moe,主线路
  - DOMAIN-KEYWORD,game,主线路
  - DOMAIN-KEYWORD,googlevideo.com,主线路
  - DOMAIN-SUFFIX,1password.com,DIRECT
  - DOMAIN-SUFFIX,vultr.com,DIRECT
  - DOMAIN-SUFFIX,mb3admin.com,DIRECT
  - DOMAIN-SUFFIX,rixcloud.io,DIRECT
  - DOMAIN-SUFFIX,tempestapp.io,DIRECT
  - DOMAIN-SUFFIX,baidu.com,DIRECT
  - DOMAIN-SUFFIX,baidu-int.com,DIRECT
  - DOMAIN-SUFFIX,erebor.douban.com,DIRECT
  - DOMAIN,mtalk.google.com,DIRECT
  - DOMAIN,alt1-mtalk.google.com,DIRECT
  - DOMAIN,alt2-mtalk.google.com,DIRECT
  - DOMAIN,alt3-mtalk.google.com,DIRECT
  - DOMAIN,alt4-mtalk.google.com,DIRECT
  - DOMAIN,alt5-mtalk.google.com,DIRECT
  - DOMAIN,alt6-mtalk.google.com,DIRECT
  - DOMAIN,alt7-mtalk.google.com,DIRECT
  - DOMAIN,alt8-mtalk.google.com,DIRECT
  - DOMAIN,alt9-mtalk.google.com,DIRECT
  - DOMAIN,captive.apple.com,DIRECT
  - DOMAIN,time-ios.apple.com,DIRECT
  - DOMAIN-SUFFIX,gateway.push-apple.com.akadns.net,DIRECT
  - DOMAIN-SUFFIX,push.apple.com,DIRECT
  - DOMAIN-KEYWORD,github,主线路
  - DOMAIN-SUFFIX,github.com,主线路
  - DOMAIN-SUFFIX,flowercloud.net,主线路
  - DOMAIN-SUFFIX,socloud.me,主线路
  - DOMAIN-SUFFIX,ytoo.asia,主线路
  - DOMAIN-SUFFIX,ytoo.co.uk,主线路
  - GEOIP,CN,DIRECT
  - MATCH,主线路
