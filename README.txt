KLC WEBSITE - GITHUB PAGES PACKAGE
==================================
Files: index.html (website), robots.txt, sitemap.xml, llms.txt, .nojekyll, set_url.py

STEP 1 - GitHub par upload (aap khud, apne account se)
  1. github.com par login karein -> New repository -> naam: klc  -> Public -> Create.
  2. "uploading an existing file" par click karein, is folder ki SAARI files drag karein
     (.nojekyll bhi) -> Commit changes.
  3. Settings -> Pages -> Source: "Deploy from a branch" -> Branch: main, folder: / (root) -> Save.
  4. 1-2 minute baad address milega:  https://AAPKA-USERNAME.github.io/klc/

STEP 2 - Address files mein daalna
  Upload se pehle ya baad mein, computer par:
     python3 set_url.py https://AAPKA-USERNAME.github.io/klc/
  Phir badli hui files dobara GitHub par upload (replace) karein.
  (Ye tool robots.txt, sitemap.xml, llms.txt aur index.html mein sahi address daal deta hai.)

STEP 3 - Google Search Console
  1. search.google.com/search-console -> Add property -> "URL prefix" -> apna GitHub address daalein.
  2. Verify ke liye "HTML tag" chunein -> meta tag mein se sirf content="..." wala code copy karein.
  3. python3 set_url.py https://AAPKA-USERNAME.github.io/klc/ YEH-CODE
     -> index.html dobara GitHub par upload karein -> Search Console mein Verify dabayein.
  4. Sitemaps -> "sitemap.xml" daalein -> Submit.
  5. URL Inspection mein apna address daal kar "Request indexing" dabayein.

Jab apna domain (.com / .pk) le lein: wahi steps dobara chalayein naye address ke saath,
GitHub Pages mein Custom domain bhi daal dein.

Office timing aur Google Maps link: index.html mein "const OFFICE={list:[...],hours:"",map:""}" mein bharein,
contact page par "Visit our office" box khud nazar aane lagega.
