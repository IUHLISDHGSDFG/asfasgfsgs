port: 7890
socks-port: 7891
allow-lan: true
mode: Rule
log-level: info
external-controller: 127.0.0.1:9090

proxies:
  - {name: "专线-Frontend","type":"vmess","server":"yyhkv2r1.cdn.node.a.ddnsdlmy.xyz","port":20313,"uuid":"e0b165f8-a014-3a69-af0d-e8b08b7fe96d","alterId":0,"cipher":"auto","udp":true,"tags":"hk","network":"ws","ws-opts":{"path":"/acaaaad0-54f5-4e10-94bb-1e6ab04649e1.y.live02.m3u8"},"skip-cert-verify":false}

  - {name: "专线-Frontend-1","type":"vmess","server":"w96y.cdn.node.a.ddnsdlmy.xyz","port":20314,"uuid":"e0b165f8-a014-3a69-af0d-e8b08b7fe96d","alterId":0,"cipher":"auto","udp":true,"tags":"hk","network":"ws","ws-opts":{"path":"/acaaaad0-54f5-4e10-94bb-1e6ab04649e1.y.live02.m3u8"},"skip-cert-verify":false}

  - {name: "专线-Frontend-2","type":"vmess","server":"78gb1.cdn.node.a.ddnsdlmy.xyz","port":20434,"uuid":"e0b165f8-a014-3a69-af0d-e8b08b7fe96d","alterId":0,"cipher":"auto","udp":true,"tags":"tw","network":"ws","ws-opts":{"path":"/acaaaad0-54f5-4e10-94bb-1e6ab04649e1.y.live02.m3u8"},"skip-cert-verify":false}

  - {name: "专线-Frontend-3","type":"vmess","server":"78gb1.cdn.node.a.ddnsdlmy.xyz","port":20435,"uuid":"e0b165f8-a014-3a69-af0d-e8b08b7fe96d","alterId":0,"cipher":"auto","udp":true,"tags":"tw","network":"ws","ws-opts":{"path":"/acaaaad0-54f5-4e10-94bb-1e6ab04649e1.y.live02.m3u8"},"skip-cert-verify":false}

  - {name: "土耳其01", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-AOOk-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其02", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-MG-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其03", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-N3-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其04", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-c-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其05", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-1Jf-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其06", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-dfL3A-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其07", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4327-orderid-10000-region-tr_adana-sessionID-XaZQc-sessiontime-5", password: "Aa112211", udp: true}
  - {name: "土耳其08", type: "socks5", server: "asdata.lumidaili.com", port: "10000", username: "userID-4558-orderid-11074-region-tr_adana-sessionID-C3l-sessiontime-5", password: "Aa112211", udp: true}
  

proxy-providers:
  主线路: {type: "http", url: "https://xiaobajie.eyedoll.site/api/v1/client/subscribe?token=6c7fb3ab868addff08d421f69ef8d4f2", interval: 86400, path: "./proxy_provider/jc.yaml", udp: false, health-check: {enable: true, interval: 600, url: "http://www.gstatic.com/generate_204"}}

proxy-groups:
  - {name: "主线路", type: "select", use: ["主线路"], health-check: {enable: true, interval: 60, url: "http://www.gstatic.com/generate_204"}}
  - {name: "消费", type: "select", proxies: ["专线-土耳其01", "专线-土耳其02", "专线-土耳其03", "专线-土耳其04", "专线-土耳其05", "专线-土耳其06", "专线-土耳其07", "专线-土耳其08"]}
  - {name: "自动切换", type: "fallback", url: "http://www.gstatic.com/generate_204", interval: 30, proxies: ["专线-Frontend", "专线-Frontend-2", "专线-Frontend-3", "专线-Frontend-1"]}
  - {name: "专线-土耳其01", type: "relay", proxies: ["自动切换", "土耳其01"]}
  - {name: "专线-土耳其02", type: "relay", proxies: ["自动切换", "土耳其02"]}
  - {name: "专线-土耳其03", type: "relay", proxies: ["自动切换", "土耳其03"]}
  - {name: "专线-土耳其04", type: "relay", proxies: ["自动切换", "土耳其04"]}
  - {name: "专线-土耳其05", type: "relay", proxies: ["自动切换", "土耳其05"]}
  - {name: "专线-土耳其06", type: "relay", proxies: ["自动切换", "土耳其06"]}
  - {name: "专线-土耳其07", type: "relay", proxies: ["自动切换", "土耳其07"]}
  - {name: "专线-土耳其08", type: "relay", proxies: ["自动切换", "土耳其08"]}
  

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
