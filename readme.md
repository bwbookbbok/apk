
zsign

disabled_func 
post_max 最大121M
nginx client_max 121M

public / 写入权限

// 对应苹果账户证书的
public/mobileprovision/embedded1.mobileprovision

// sign ssl证书需要nginx, apache
openssl rsa -in mbaike.key -out mbaikenopass.key

openssl smime -sign -in /home/wwwroot/apk/public/ios_describe_aoi/52.mobileconfig -out /home/wwwroot/apk/public/ios_describe/52.mobileconfig -signer /home/wwwroot/apk/public/sign/mbaike.crt -inkey /home/wwwroot/apk/public/sign/mbaikenopass.key -certfile /home/wwwroot/apk/public/sign/ca-bundle.pem -outform der -nodetach

zsign  -c /home/wwwroot/apk/public/spcer/26certificate.pem -k  /home/wwwroot/apk/public/spcer/26key.pem -m  /home/wwwroot/apk/public/ios_movileprovision/00008020-000B34813612002E.mobileprovision  -o  /home/wwwroot/apk/public/upload/super_signature_ipa/demo.ipa /home/wwwroot/apk/public/upload/super_signature/20200701/a7971abb4134fc0cfcec7d589e1ebcf6.ipa
