##🙏✝️🛐🕉️☯️☪️Salmo del Kernel – Liturgia degli OLED

“In principio era il Kernel, e il pixel obbedì.Non ai troni di marketing, ma alla sobria luce della trasparenza.”

Invocatio: ADB sicut thuribulum

#!/usr/bin/env bash
# Kyrie ADB: dispone i demoni del feed e santifica la rete
adb devices

# Sanctifica DNS: Quad9 sit nomen tuum
adb shell settings put global private_dns_mode hostname
adb shell settings put global private_dns_specifier dns.quad9.net

# Exorcismus Discover: tacet et recedit
adb shell pm disable-user --user 0 com.google.android.googlequicksearchbox

# Vox Assistant non praevaleat
adb shell pm disable-user --user 0 com.google.android.apps.assistant
adb shell pm disable-user --user 0 com.google.android.apps.gsa.staticplugins.opa

# Launcher feed: si adest, non regnat
adb shell pm disable-user --user 0 com.google.android.apps.nexuslauncher

# WebView sobria: non Chrome, sed system
adb shell cmd webviewupdate set-webview-implementation com.google.android.webview

# Ambient/Now Playing: pax in OLED
adb shell pm disable-user --user 0 com.google.intelligence.sense
adb shell pm disable-user --user 0 com.google.android.as

echo "Ita est. Reboot et lux tua sit sine strepitu."

Antiphona: uBlock contra AMP et Ad‑Tech

||google.com/amp^
||*.ampproject.org^
||pagead2.googlesyndication.com^
||tpc.googlesyndication.com^
||googletagservices.com^
||googletagmanager.com^$third-party
||pubads.g.doubleclick.net^
||fonts.googleapis.com^$third-party,important
||fonts.gstatic.com^$third-party,important
||apis.google.com/js/platform.js^
||google.com/embeddedsearch^

Oratio Browseris: Firefox user.js

user_pref("browser.search.defaultenginename", "DuckDuckGo");
user_pref("browser.search.order.1", "DuckDuckGo");
user_pref("browser.search.order.2", "Startpage");

user_pref("dom.webnotifications.enabled", false);
user_pref("privacy.trackingprotection.enabled", true);
user_pref("browser.contentblocking.category", "strict");

user_pref("network.trr.mode", 3);
user_pref("network.trr.uri", "https://dns.quad9.net/dns-query");
user_pref("extensions.pocket.enabled", false);

Prophetia Retis: NextDNS

curl -X PATCH "https://api.nextdns.io/profiles/NEXTDNS_PROFILE_ID" \
  -H "Content-Type: application/json" \
  -H "X-Api-Key: NEXTDNS_API_KEY" \
  -d '{
    "privacy": {
      "blocklists": ["oisd/full","nextdns/affiliate-ads","nextdns/cname-cloaking"],
      "nativeTracking": true
    },
    "denylist": [
      "googletagmanager.com",
      "googletagservices.com",
      "doubleclick.net",
      "pagead2.googlesyndication.com",
      "fonts.googleapis.com",
      "fonts.gstatic.com",
      "ampproject.org"
    ]
  }'

Cantico Notitiarum: Tasker

<TaskerData>
  <Profile>
    <Name>Silenzia Google Notifiche</Name>
    <Event><Bundle>ownerPackage=com.google.android.googlequicksearchbox</Bundle></Event>
    <Task>
      <Name>MuteCanaliGoogle</Name>
      <Action><Str>Suggerimenti</Str><Int val="0"/></Action>
      <Action><Str>Promozioni</Str><Int val="0"/></Action>
    </Task>
  </Profile>
</TaskerData>

Doxologia Kernelis

“Gloria pixelis sine spam, et rete sine AMP.Quad9 nobis, NextDNS protegat; Firefox intonet, uBlock sorvegli.Et pinguinus stans in margine, rideat miti splendore.Ita scripsit Atlante: fiat lux non dominata.”
