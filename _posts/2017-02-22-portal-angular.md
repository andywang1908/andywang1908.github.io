
#blockchain 

##ref

[R1](https://www.zhihu.com/question/37290469)

[R2](https://www.zhihu.com/question/27687960)

[R3](http://www.bnext.com.tw/ext_rss/view/id/1336998)

[R4](https://rocket.cafe/talks/58431)



wcm config poc theme


http://localhost:10039/sodp/mypoc/s2i?uri=s2i:IACInfo
http://10.160.200.14:10039/sodp/mypoc/s2i?uri=s2i:IACInfo

http://localhost:10039/sodp/portal/s2i
http://10.160.200.14:10039/sodp/portal/s2i
http://10.160.200.14:10039/sodp/myportal/s2i/Applications/Content/Authoring

https://localhost:10041/ibm/console/login.do?action=secure
http://10.160.200.4:10041/wps/portal

https://10.160.200.14:10041/sodp/portal            WebSphere_Portal   server1       /home/andy/IBM/WebSphere/wp_profile/PortalServer
https://10.160.200.6:10041/sodp/myportal

http://localhost:10039/sodp/myportal
http://localhost:10039/sodp/portal

http://10.160.200.6:10039/sodp/portal/s2i
http://10.160.200.6:10039/sodp/portal/s2i/!ut/p/z1/04_Sj9CPykssy0xPLMnMz0vMAfIjo8ziDVCAo4FTkJGTsYGBu7OJfjghBVEY0sgKgfqjsChBmOBvhFUBihkFuREGmY6KigC8rV5c/dz/d5/L2dBISEvZ0FBIS9nQSEh/
http://localhost:10039/sodp/portal/s2i/!ut/p/z1/04_Sj9CPykssy0xPLMnMz0vMAfIjo8ziDVCAo4FTkJGTsYGBu7OJfjghBVEY0sgKgfqjsChBmOBvhFUBihkFuREGmY6KigC8rV5c/dz/d5/L2dBISEvZ0FBIS9nQSEh/

https://localhost:10041/ibm/console/logon.jsp
https://10.160.200.14:10041/ibm/console/logon.jsp

ports
SOAP_CONNECTOR_ADDRESS  ubuntu  10033  No associated transports  

10033   8880
ubuntu  10.160.200.14

http://10.160.200.6:10039/s2iThemeStatic/themes/s2i/css/s2i/s2i.desktop.css

???
real node_modules must be in parent folder
when to use parent folder , sometimes can ref, sometimes can not.
???


ng serve --host 0.0.0.0 --port 4200
copy @s2i
npm install @angular/cli@^1.0.0-rc.2 -g
npm install gulp@^2.2.4@^3.9.1 -g
export PATH=/home/andy/ins/sp_cmdln:$PATH
echo $PATH
change host
sudo npm cache clean
npm link ng2-s2i-common
ln -s ../node_modules node_modules  
ln -s /home/andy/ccc/node_modules node_modules
export PATH=$PATH:/home/andy/ccc/ng2-s2i-cart/node_modules/.bin

- svn co --username ebc\wangan1 https://gscbiqdcapmdw01.cihs.ad.gov.on.ca:8443/svn/SOIT_S2I_Portal/branches/angular2/s2i-angular2-v3

------build
npm run build:prod

npm install --production
npm install @angular/cli@^1.0.0-rc.2 --save-dev

npm install assets-webpack-plugin --save-dev
npm install copy-webpack-plugin --save-dev
npm install awesome-typescript-loader@^2.2.4 --save-dev     #TODO change to code to update to latest
npm install script-ext-html-webpack-plugin --save-dev
npm install webpack-md5-hash --save-dev
npm install v8-lazy-parse-webpack-plugin --save-dev
npm install angular2-template-loader --save-dev

npm install angular2-router-loader --save-dev
npm install ng2-translate --save-dev
npm install ts-helpers --save-dev
npm install @types/express --save-dev
npm install @types/source-map --save-dev
npm install @types/uglify-js --save-dev
npm install @types/webpack --save-dev
npm install @types/jasmine --save-dev
npm install @types/selenium-webdriver --save-dev


npm uninstall @types/jasmine --save-dev
npm install @types/jasmine@2.5.38 --save-dev
#why not ok on @2.5.46   wired @1.* at first time

--------push
npm run build:prod
npm run sp-push

W:\svn\angular\s2i-angular2-v4\s2i-build\tools\config\s2i-project.config.ts:
   22    S2I_COMMON_THEME_DIR = './dist/common_theme';
   23    PORTAL_CONFIGURATION: PortalConfiguration = {
   24:     CONFIG_URL: 'http://10.160.200.6:10039/sodp/config',
   25:     SP_SERVER: 'http://10.160.200.6:10039',

s2i-cart-iac


npm install gulp --save-dev # need,  not need do first

npm install ts-node --save-dev

npm install run-sequence --save-dev
npm install slash --save-dev
npm install browser-sync --save-dev
npm install express-history-api-fallback --save-dev
npm install open --save-dev
npm install gulp-load-plugins --save-dev
npm install shelljs --save-dev

#TypeError: Cannot read property 'compile' of undefined
npm install handlebars --save-dev       




-------- type/jasmine     ../node_modules


cd /home/andy/ddd/s2i-build
cd ../ng2-s2i-cart
ln -s /home/andy/ddd/node_modules node_modules   
cd ../ng2-s2i-common
ln -s /home/andy/ddd/node_modules node_modules
cd ../s2i-build
ln -s /home/andy/ddd/node_modules node_modules
cd ../s2i-cart-iac
ln -s /home/andy/ddd/node_modules node_modules
cd ../s2i-landing
ln -s /home/andy/ddd/node_modules node_modules
cd ../s2i-receipt-iac
ln -s /home/andy/ddd/node_modules node_modules
cd ../s2i-theme-header
ln -s /home/andy/ddd/node_modules node_modules
cd ../s2i-web-iac
ln -s /home/andy/ddd/node_modules node_modules



cd /home/andy/ccc/s2i-build/node_modules
unlink ng2-s2i-common
unlink ng2-s2i-common
ln -s /home/andy/ccc/ng2-s2i-common ng2-s2i-common
ln -s /home/andy/ccc/ng2-s2i-cart ng2-s2i-cart

ln -s /home/andy/ccc/node_modules node_modules  or
ln -s ../node_modules node_modules



----- ng2-s2i-cart         error of obverve

1. set path=c:\workspaces_angular\s2i\node_odules\.bin;%path%
2. npm run compile
3. npm run buildWindow on windows or npm run build on linux
4. copy files under dist diretory under node-modules/@s2i/cart


export PATH=$PATH:/home/andy/ddd/ng2-s2i-cart/node_modules/.bin
ln -s /home/andy/ddd/node_modules node_modules   




ERROR in /home/andy/ddd/s2i-web-iac/src/app/iac/iac.component.ts (183,5): Type 'FormGroup' is not assignable to type 'FormGroup'.
  Types of property 'controls' are incompatible.
    Type '{ [key: string]: AbstractControl; }' is not assignable to type '{ [key: string]: AbstractControl; }'.
      Index signatures are incompatible.
        Type 'AbstractControl' is not assignable to type 'AbstractControl'.
          Types have separate declarations of a private property '_valueChanges'.)


npm install @types/hammerjs --save-dev             find missing module by npm compile in ng2 folder!!!!


find by '@s2i/common'   '@s2i/cart' 

// from '@s2i/cart'; or from 'ng2-s2i-cart/src/cart';

// from '@s2i/common'; or from 'ng2-s2i-common/src/common/translate/translate.service';
// from '@s2i/common'; or from 'ng2-s2i-common/src/common';





------ return value

                let observable: Observable<Response> =
                  this.http.request(req);
              try {

                observable = this.handleResponse(
                  observable, descriptor.isJSON);

                // intercept the response
                if (observable != undefined) {
                  observable = this.responseInterceptor(observable);
                }
              } catch (error) {
                console.log(">>>>>>>>>>>>>>>>>1<<<<<<<<<<<<<<<<<");
                console.log(error);
                this.handleError(error);
              }
                return observable;




svn propset svn:ignore node_modules .
svn propedit svn:ignore .

export SVN_EDITOR=vi


If your directory foo is already under version control, remove it first with:

svn rm --keep-local node_modules
...then ignore:

svn propset svn:ignore node_modules .


svn ignore 的用法（忽略文件及目录）
若想创建了一个文件夹，并且把它加入版本控制，但忽略文件夹中的所有文件的内容：
$ svn mkdir node_modules 
# cd node_modules
$ svn propset svn:ignore '*' node_modules 
$ svn ci -m 'V4'
若想创建一个文件夹，但不加入版本控制，即忽略这个文件夹：
$ mkdir spool 
$ svn propset svn:ignore 'spool' . 
$ svn ci -m 'Ignoring a directory called "spool".'
若已经创建了文件夹，并加入了版本控制，现在想忽略这个文件夹，但要保持文件夹的内容：
$ svn export spool spool-tmp 
$ svn rm spool 
$ svn ci -m 'Removing inadvertently added directory "spool".' 
$ mv spool-tmp spool 
$ svn propset svn:ignore 'spool' . 
$ svn ci -m 'Ignoring a directory called "spool".'




------- global

sudo npm proxy -g
sudo npm install -g @angular/cli
# no need? since ng-cli is there .   
sudo npm install -g webpack

------- add user
sudo adduser allen


cd /home/allen/svn/angular/s2i-angular2-v4/s2i-build

svn co --username ebc\wangan1 https://gscbiqdcapmdw01.cihs.ad.gov.on.ca:8443/svn/SOIT_S2I_Portal/branches/angular2/s2i-angular2-v4

svn co --username ebc\wangan1 https://gscbiqdcapmdw01.cihs.ad.gov.on.ca:8443/svn/SOIT_S2I_Portal/branches/angular2/mockApi



cd s2i-build
#mkdir ../node_modules

cd ../s2i-build
unlink node_modules
ln -s ../node_modules node_modules
cd ../s2i-cart-iac
unlink node_modules
ln -s ../node_modules node_modules
cd ../s2i-landing
unlink node_modules
ln -s ../node_modules node_modules
cd ../s2i-receipt-iac
unlink node_modules
ln -s ../node_modules node_modules
cd ../s2i-theme-header
unlink node_modules
ln -s ../node_modules node_modules
cd ../s2i-web-iac
unlink node_modules
ln -s ../node_modules node_modules

cd node_modules
mkdir @s2i
cd @s2i

ln -s ~/svn/angular/s2i-angular2-v4/ng2-s2i-common/src/common common
ln -s ~/svn/angular/s2i-angular2-v4/ng2-s2i-cart/src/cart cart  

vi ~/.curlrc
proxy = http://204.40.194.129:3128

git config --global http.proxy http://ebc%5Cwangan1:Ontario7%24@204.40.194.129:3128

vi ~/.subversion/config
global-ignores = *.o *.lo *.la *.al .libs *.so *.so.[0-9]* *.a *.pyc *.pyo __pycache__ __node_modules__ node_modules__ node_modules


cd ~/svn/angular/s2i-angular2-v4/s2i-web-iac
npm install
ng serve --host 0.0.0.0 --port 4280
ng serve --host 0.0.0.0 --port 4280 --proxy-config proxy.service.json

sudo smbpasswd -a           mock
sudo service smbd restart
may need restart windows for changing password

working and verify

- svn revert -R .
- svn up .
- svn commit -m "v5"
- svn commit . -m 'ip address'
- svn add * --force



sudo npm install forever -g
cd /home/mock/svn/mock/mockApi
forever start bin/www
forever stop bin/www




            <div class="Instructions" id="breadcrums">
                
                        <a href='/s2i_survey_admin/home'>Home</a><span><span>&gt;</span></span>
                       
                        <span>My Surveys (JennTest)</span>
                                    
            </div>


http://10.160.200.145:4280/s2i/iac/api/v1/verifications Failed to load resource: the server responded with 

http://10.160.200.145:10039/api/s2i/iac/api/v1/orderitems/12


http://10.160.200.145:10039/s2i/iac/api/v1/verifications

http://10.160.200.145:4280/s2i/iac/api/v1/orderitems/33
http://10.160.200.145:10039/s2i/iac/api/v1/orderitems/33
http://10.160.200.145:4280/s2i/iac/api/v1/orderitems/33 


  // /api/s2i/hello
  // /api/s2i/iac/api/v1/providers
  verify(iacOrderItem: IacOrderItem) {
    var iacOrderItemClone: any = Object.assign({}, iacOrderItem);

    //private obs: Observable<any>;
    //iacOrderItem = <IacOrderItem>{};
    /**/
    this.iacClient.verify(iacOrderItem)
      .subscribe(
        data => {
          this.ngRedux.dispatch({
            type: IacActions.ACTION_VERIFY,
            payload: iacOrderItemClone
          });
          console.log('andy data::' + JSON.stringify(data));
        },
        err => {
          this.ngRedux.dispatch({
            type: IacActions.ACTION_VERIFY_FAIL,
            payload: iacOrderItemClone
          });
          console.log('andy err:' + JSON.stringify(err));
        }
      );
  }




  // @GET("/s2i/hello")
  @GET('/s2i/iac/api/v1/orderitems/{itemId}')
  @Produces(MediaType.JSON)
  getOrder(@Path('itemId') itemId: string): Observable<models.IacOrderItem> {
    return null;
  }

  // /api/s2i/hello
  // /api/s2i/iac/api/v1/providers
  // https://angular.io/docs/ts/latest/api/http/index/RequestOptions-class.html
  getProviders(): Observable <any> {

    let headers = new Headers();
    // headers.append('mock-error-code', '403');
    headers.append('Authorization', 'true'); 

    var options = new RequestOptions({
      method: RequestMethod.Get,
      url: '/api/s2i/hello',
      headers : headers
    });

    let req = new Request(options);
    // let observable: Observable<Response> = this.http.request(req);
    // handleResponse

    return this.http.request(req)
      // .timeout(30000, new Error('Timeout has occurred.'))
      .map((res) => {
        // console.log('res:' + JSON.stringify(res));
        return res.text();
        // return res.json();
      });




http://swagger.io/swagger-editor/
http://editor.swagger.io/#/







https://developer.ibm.com/answers/questions/175838/why-does-portal-server-fail-to-start-after-install.html

https://www-10.lotus.com/ldd/portalwiki.nsf/xpDocViewer.xsp?lookupName=Combined+Cumulative+Fix+Readme+V8.5.0.0#action=openDocument&res_title=IBM_WebSphere_Portal_V8.5.0.0_combined_cumulative_fix_instructions_standalone_cf8500&content=pdcontent




##### Change Context Root



delete your RSA portal server, apply context change, then new RSA portal server again  
Allways make sure WAS > Enterprise Applications > wps > Startup behavior > Startup order = 10  
The value can be reset to 1 by RSA, it stores as startingWeight="10" in:  
C:\IBM\WebSphere\wp_profile\config\cells\ond2c00802001\applications\wps.ear\deployments\wps\deployment.xml



......remote debug
http://stackoverflow.com/questions/9028984/how-do-you-connect-an-eclipse-to-a-websphere-application-server-hosted-on-remote

......remote server        impossible?

https://www.genuitec.com/products/myeclipse/learning-center/websphere/remote-websphere-connectors/

Remote WebSphere Connectors

http://stackoverflow.com/questions/39396604/cant-connect-remotely-to-was-8-5-full-profile-installed-on-ubuntu-14-04-from-ra



/home/andy/IBM/WebSphere/AppServer/profiles/cw_profile
/home/andy/IBM/WebSphere/AppServer/profiles/AppSrv01
/home/andy/IBM/WebSphere/wp_profile/PortalServer       working on Eclipse
/home/andy/IBM/WebSphere/wp_profile          working on RSA

CTGRI0007E An error occurred when reading the remote file named /home/andy/IBM/WebSphere/wp_profile/PortalServer/config/cells .


CTGRI0007E An error occurred when reading the remote file named /home/andy/IBM/WebSphere/wp_profile/PortalServer/config/cells .

https://books.google.ca/books?id=oBnCAgAAQBAJ&pg=PA1821&lpg=PA1821&dq=server+profile+path+portal&source=bl&ots=kTFNqxnpCF&sig=O31bwGhs1wFPeMA-3bTTIqhfD5U&hl=en&sa=X&ved=0ahUKEwjj44TP1PnSAhVM9YMKHYIXC40Q6AEIRjAI#v=onepage&q=server%20profile%20path%20portal&f=false

Rational Application Developer for WebSphere Software V8 Programming Guide      good book

The following problems has occurred when starting the server.
The server may not be started in the correct mode.  You can restart the server to desired mode if it is started.
CTGRI0075E A file transfer to or from the system named [10.160.200.14]  timed out before the transfer could complete. The current timeout interval is set to 240000 milliseconds, and might need to be increased.

ADMU0116I: Tool information is being logged in file
           /home/andy/IBM/WebSphere/wp_profile/logs/WebSphere_Portal/startServer.log
ADMU0128I: Starting tool with the wp_profile profile
ADMU3100I: Reading configuration for server: WebSphere_Portal
ADMU3200I: Server launched. Waiting for initialization status.


open remote debug 7777


virtual portal  s2i
s2i.angular.theme.skin.Standard

https://www.ibm.com/support/knowledgecenter/SSYJ99_8.5.0/dev-theme/themeopt_themedev_manual_deployregister.html  theme


portal setting import xml
http://www.webportalclub.com/2013/04/using-xml-access-to-export-and-import.html     import setting


https://www-10.lotus.com/ldd/portalwiki.nsf/dx/How_to_develop_your_own_custom_portal_8.5_theme.    theme develop

https://developer.ibm.com/digexp/blog/2015/05/26/developing-ibm-websphere-portal-8-5-ear-themes-a-step-by-step-guide/   theme develop


https://www.slideshare.net/michelebuccarello/custom-theme-creation-websphere-portal-85      save life


ear 10+1

portlet  Web Content Management - ML Library Copy     JSR 286


 
!!!
https://www.ibm.com/support/knowledgecenter/en/SS3JLV_8.0.0/wcm/wcm_config_wcmlibrary_export.html
Resources > Resource Environment > Resource Environment Providers > WCM WCMConfigService > Custom properties.


must as admin
cd C:\IBM\WebSphere\wp_profile\ConfigEngine
ConfigEngine.bat export-wcm-data -DWasPassword=admin -DPortalAdminPwd=admin
ConfigEngine.bat export-wcm-data -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i

ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent.zip -DLibraryName="Web Content" -DWasPassword=mypassword -DPortalAdminPwd=mypassword -DVirtualPortalHost=vp.example.com

ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent.zip -DLibraryName="Web Content" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i


ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent.zip -DLibraryName="Portal Site" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i
ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent1.zip -DLibraryName="s2i-apps" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i


./ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent1.zip -DLibraryName="s2i-apps" -DLibraryTitle="s2i-apps title" -DLibraryDescription="s2i-apps desc" -DLibraryNameTextProvider=provider -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i


http://10.160.200.184:8080/mock/login.html



ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent.zip -DLibraryName="Web Resources v70" -DWasPassword=admin -DPortalAdminPwd=admin

./ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent.zip -DLibraryName="Web Resources v70" -DLibraryTitle="Web Resources v70 title" -DLibraryDescription="Web Resources v70 desc" -DLibraryNameTextProvider=provider -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en -DWasPassword=admin -DPortalAdminPwd=admin






-------portal    application



init  1 of 6  Next >  Total 114    application

--0.add virtual portals s2i
a.select user by search

--1.theme
intall ear
import 2 theme xml

--2.ear
a.s2i-* 6 apps
b.TODO other

AjaxProxy_war
PA_WCMMLLibraryCopy       wcm-ml-librarycop_war
  S2I_SODPUtilEAR
WCM_Multilingual      (fail?)

--3. wcm
export PATH=/home/andy/ins/sp_cmdln:$PATH

/opt/IBM/WebSphere/ConfigEngine/ConfigEngine.sh
/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh    should this
/opt/IBM/WebSphere/AppServer/profiles/cw_profile/ConfigEngine/ConfigEngine.sh



/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh export-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent.zip -DLibraryName="Web Resources v70" -DWasPassword=admin -DPortalAdminPwd=admin


/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent.zip -DLibraryName="Portal Site" -DLibraryNameTextProvider=provider -DWasPassword=admin -DVirtualPortalContext=s2i -DPortalAdminPwd=admin -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en
/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent1.zip -DLibraryName="ML Configuration" -DLibraryNameTextProvider=provider -DWasPassword=admin -DVirtualPortalContext=s2i -DPortalAdminPwd=admin -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en
/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent2.zip -DLibraryName="s2i-apps" -DLibraryNameTextProvider=provider -DWasPassword=admin -DVirtualPortalContext=s2i -DPortalAdminPwd=admin -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en
/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent3.zip -DLibraryName="Script Application Library" -DLibraryNameTextProvider=provider -DWasPassword=admin -DVirtualPortalContext=s2i -DPortalAdminPwd=admin -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en
/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent4.zip -DLibraryName="Site Builder Template Library" -DLibraryNameTextProvider=provider -DWasPassword=admin -DVirtualPortalContext=s2i -DPortalAdminPwd=admin -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en
/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent5.zip -DLibraryName="s2i-config" -DLibraryNameTextProvider=provider -DWasPassword=admin -DVirtualPortalContext=s2i -DPortalAdminPwd=admin -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en
/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent6.zip -DLibraryName="s2i-resource-en" -DLibraryNameTextProvider=provider -DWasPassword=admin -DVirtualPortalContext=s2i -DPortalAdminPwd=admin -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en
/opt/IBM/WebSphere/wp_profile/ConfigEngine/ConfigEngine.sh import-library-copy -DLibraryPath=/home/andy/wcm_import/webcontent7.zip -DLibraryName="s2i-resource-fr" -DLibraryNameTextProvider=provider -DWasPassword=admin -DVirtualPortalContext=s2i -DPortalAdminPwd=admin -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en


---------------
windows admin!!

C:\IBM\WebSphere\ConfigEngine\ConfigEngine.bat
C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat     working
C:\IBM\WebSphere\AppServer\profiles\cw_profile\ConfigEngine\ConfigEngine.bat

admin!!    

C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent.zip -DLibraryName="Portal Site" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i
C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent1.zip -DLibraryName="ML Configuration" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i
C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent2.zip -DLibraryName="s2i-apps" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i
C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent3.zip -DLibraryName="Script Portlet Library" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i
C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent4.zip -DLibraryName="Site Builder Template Library" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i
C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent5.zip -DLibraryName="s2i-config" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i
C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent6.zip -DLibraryName="s2i-resource-en" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i
C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat export-library-copy -DLibraryPath=C:\wcm_export\webcontent7.zip -DLibraryName="s2i-resource-fr" -DWasPassword=admin -DPortalAdminPwd=admin -DVirtualPortalContext=s2i


C:\IBM\WebSphere\wp_profile\ConfigEngine\ConfigEngine.bat import-library-copy -DLibraryPath=C:\wcm_export\webcontent5.zip -DLibraryName="s2i-config-andy" -DLibraryNameTextProvider=provider -DVirtualPortalContext=s2i -DWasPassword=admin -DPortalAdminPwd=admin -DLibraryNameTextProviderKey=key -DLibraryBaseLocale=en


--make library visiable
https://www.ibm.com/support/knowledgecenter/en/SSHRKX_8.5.0/help/panel_help/wcm_config_authoringportlet_libraries.html
Portal User Interface > Manage Pages > unique name: com.ibm.wps.hiddenpage.wcm.Authoring_Portlet

working
Preferences  Configure   Edit Shared Settings

import derby

cd C:\Users\WangAn1\Downloads
java -jar squirrel-sql-3.7.1-standard.jar



-- wcm manully

Script Application (Script Portlet)             ?     in  Script Application Library


-- classpath


/opt/IBM/SODP/andy/s2i-common-0.0.1-SNAPSHOT.jar            !!!!      ????




-- about   presantation template
a.define in parent node
b.overide in at advanced option
c.create clean library so where is only one pt


-- wcm login
a.content acess
b.at pt access
c.libary access



theme.html
  <a rel="dynamic-content" href="dyn-cs:id:st_wcm_content?path=s2i-apps/theme/common"></a>
wcm
[Plugin:S2iCommonContextRenderingPlugin][Plugin:ThemeComponent component="polyfills"][Plugin:ThemeComponent component="vendor"]

reason: author fileter

https://developer.ibm.com/digexp/blog/2015/10/01/sample-custom-scripted-wcm-plugins/  example





skin.html
                <h2 class="dndHandle" draggable="true" ondragstart="wpModules.dnd.util.portletDragStart(event, this, this.parentNode, 30, 0);"
                    ondragend="wpModules.dnd.util.portletDragEnd(event);">
                    <!-- The "lm:title" dynamic spot is used for dynamic title support. -->
                    <span class="lm-dynamic-title a11yRegionLabel ac-title-b"><a rel="dynamic-content" href="lm:title"></a></span>
                </h2>

reason: content link is not right




???????????get target 
wcm config poc theme



S2iProductContextRenderingPlugin

  public boolean render(final RenderingPluginModel p_model) throws RenderingPluginException {

    
    final Writer writer = p_model.getWriter();
    try {
      writer.write(S2iRestUtils.instance().getProductJavascriptContext((HttpServletRequest)p_model.getRequest()));
      
    } catch (Exception e) {
      e.printStackTrace();
    } 

    return false;
  }


S2iRestUtils
    public String getProductJavascriptContext

    s2i_context.productInfoUrl = '


S2iApplicationRenderingPlugin

S2iRestUtils
    getApplicationContextPath

Libraries>s2i-apps>Content>S2I Products>s2i-landing

<htmlwrapper>
    <div><s2i-landing-root><div style="display:none">If you see this text. It means theme are not deployed properly, or Quotes application does not run well on this theme.</div></s2i-landing-root></div>
      <script type="text/javascript" src="/sodp/wcm/myconnect/s2i/s2i-apps/resource-bundles/s2i-resources?SRV&#x3D;cmpnt&cmpntname&#x3D;s2i-resource.js&source&#x3D;content&subtype&#x3D;javascript&s2i-resource=/common/product-status-resources"></script>
      <script type="text/javascript" src="[Plugin:ScriptPortletElementURL element="s2i-landing.js"]"></script>      
    
</htmlwrapper>


https://www.houzz.com/pro/bruceatwalden/walden-homes
http://www.bhg.com/rooms/rooms/basement/transforming-basement-into-family-room/


https://www.ibm.com/support/knowledgecenter/en/SSDK36_8.5.0/dev-portlet/csa2r_dyn_cntnt_spot.html

W:\SODP\Apps\S2I\Logs\s2i-poc.log


s2i-apps/s2i-products/s2i-landing




[5/2/17 14:21:37:335 EST] 0000014a ExceptionLogg W com.ibm.wps.logging.ExceptionLogger logThrowable An exception occurred: [No page defined for ca.on.gov.s2i.page.product.info]. Enable traces for [com.ibm.wps.logging.ExceptionLogger=all] to see the exception stack trace.




https://developer.ibm.com/digexp/docs/docs/themes/displaying-dynamic-portlet-titles-portal-8-5/   portal title


https://www-10.lotus.com/ldd/portalwiki.nsf/xpDocViewer.xsp?lookupName=IBM+Web+Content+Manager+7+Product+Documentation#action=openDocument&res_title=Selecting_a_JSP_file_wcm7&content=pdcontent

within any other web application running on portal. When referencing JSP files in another web application, use the following path: contextPath;jspPath
For example: /wps/customapplication;/jsp/editor.jsp

/s2i/wcm;/jsp/S2iOperationInfo.jsp
http://10.160.200.68:10039/s2i/wcm

Working directory:C:/WebSphere/SODP/Apps/S2I
Product Config:ca.on.gov.s2i.config.impl.S2iProductConfigImpl@72a66f4c
Product Family:ca.on.gov.s2i.config.impl.S2iProductFamilyConfigImpl@500456c3
product info:s2i-apps/s2i-products/s2i-landing
form-app:s2i-apps/s2i-products/iac/iac/s2i-web-iac
s2i_context.productScriptBaseUrl = 'null';
s2i_context.s2iServiceBaseUrl = 'null';
s2i_context.restServiceBaseUrl = 'null';
s2i_context.tooltip-en = 'tooltip-en';
s2i_context.tooltip-fr = 'tooltip-fr';
s2i_context.page.id = 'ca.on.gov.s2i.page.product.info';
s2i_context.window.id = 'ca.on.gov.s2i.window.product.info';
s2i_context.app-content-path = '/iac/iac/iac-resources';
s2i_context.productTitleEn = 'Integrated Address Change';
s2i_context.productTitleFr = 'Changement d'adresse intégré';
s2i_context.supressTopNav = show;


<script>s2i_context.opInfo = {"productCode":null,"noOrderNowMsg":"","productMsg":"","productAvailable":true,"cartFull":false,"orderItemFull":false,"bypassProductInfo":false,"productUrl":null,"proceedUrl":null};console.log('s2i application context created:');</script>

Enterprise Applications > s2i-wcm-ear > Context Root For Web Modules     /s2i/wcm


s2i-resources:260              s2i resource bundle created


var s2i_app_bundle =IWKWC0031E: Content item not found s2i-resource-en/resource-bundles/common/product-status-resources.;var s2i_theme_bundle =IWKWC0031E: Content item not found s2i-resource-en/resource-bundles/theme/theme-resources.;var s2i_common_bundle =IWKWC0031E: Content item not found s2i-resource-en/resource-bundles/common/common-resources.;var s2i_bundle = Object.assign({}, s2i_theme_bundle, s2i_common_bundle, s2i_app_bundle);S2i.s2i_bundle = s2i_bundle;console.log('s2i resource bundle created');console.log(s2i_bundle);



eng and french
hide button such as workflow
disable workflow
s2i-theme-footer/s2i-theme-footer.js   s2i-theme-footer--s2i-theme-footer.js in s2i-apps  -> Theme -> theme   &  theme-2-2-1


script --->  s2i-app ---> s2i-resouce



5000K Daylight White Decorative Candle Light Bulb E12 Base, B11 Led Light Bulbs



