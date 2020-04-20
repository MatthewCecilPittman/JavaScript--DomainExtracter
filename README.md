# JavaScript--DomainExtracter
Codewars Domain Extractor solution

function domainName(url){
  let arr;
  if (/www/.test(url)) {
    arr = url.split('.');
    return arr[1];
  } else if (/http/.test(url)) {
    arr = url.split('//');
    arr = arr[1].split('.');
    return arr[0];
  } else {
    arr = url.split('.');
    return arr[0];
  }
} 



try the test below
------------------------
domainName("http://google.co.jp")
