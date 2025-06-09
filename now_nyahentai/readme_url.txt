re2289732_feed.xml -> https://nyahentai.re/magazine/re2289732/feed/
re2289732_embed.json -> https://nyahentai.re/wp-json/oembed/1.0/embed?url=https://nyahentai.re/magazine/re2289732/
settings.json -> https://nyahentai.re/wp-json/
user_list.json -> https://nyahentai.re/wp-json/wp/v2/users
plugin_list.txt -> `curl -H 'Cache-Control: no-cache, no-store' -L -ik -s https://nyahentai.re | grep -E 'wp-content/plugins/' | sed -E 's,href=|src=,THIIIIS,g' | awk -F "THIIIIS" '{print $2}' | cut -d "'" -f2`
pages_list.json -> https://nyahentai.re/wp-json/wp/v2/pages
all_methodlist.xml -> curl -X POST https://nyahentai.re/xmlrpc.php -H "Content-Type: text/xml" -d '<?xml version="1.0"?><methodCall><methodName>system.listMethods</methodName><params></params></methodCall>'