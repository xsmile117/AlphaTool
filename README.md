# AlphaTool
Python下带session的urllib网页操作封装类


Example

myHttp=myHttp.MySession()
loginURL = "http://XXXX"
loginheaders = {"Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
               "Accept-Encoding": "gzip,deflate,sdch",
               "Accept-Language": "zh-CN,zh;q=0.8",
               "Host": "32.0.249.1",
               "Origin": "http://XXXXX",
               "Referer": "http://XXXX",
               "User-Agent": "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/35.0.1916.153 Safari/537.36",
               "Connection": "keep-alive"}
values = {'user': checkuser, 'pass': checkuserpassword}
postdata = urllib.parse.urlencode(values) 
page_code, page = myHttp.post(loginURL, postdata, loginheaders)
