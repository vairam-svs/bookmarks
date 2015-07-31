MVC Routers and Handlers: 
http://haacked.com/archive/2008/04/10/upcoming-changes-in-routing.aspx/
http://haacked.com/archive/2008/07/14/make-routing-ignore-requests-for-a-file-extension.aspx/

routes.IgnoreRoute("{*allaspx}", new {allaspx=@".*\.aspx(/.*)?"});
routes.IgnoreRoute("{*favicon}", new {favicon=@"(.*/)?favicon.ico(/.*)?"});

