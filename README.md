使用 [nhjr-make_ccx](https://github.com/NanHaiJuRuo/nhjr-make_ccx) 作为扩展打包器。  
该扩展使用了隐藏积木作为缓存，以保存到作品。
***

### 目前已通过以下测试：  
[]()
✅输入不支持的列表，或不是列表的内容时，自动抛出错误并停止运行对应积木。  
✅扩展加载测试通过。  
✅删除所有自定义菜单时，自动删除项目文件里的缓存。  
✅多次测试各种情况后，未出现损坏作品的情况。  

***
### 扩展加载测试：
[]()
✅可以正常启用。  
✅启用后自动完成缓存读取。  
✅卸载后再装载后，积木列表不会缺失，功能照常使用。  
✅未装载扩展时上传作品，自动完成缓存读取、装载，并刷新积木列表。  
✅装载状态下上传作品，自动完成缓存读取，并刷新积木列表。  
✅将作品文件的JSON手动更改后，不会导致编辑器损坏（但可能会导致作品不能正常运作，所以别乱改）。  
[]()    原理：若整个菜单不符合clipcc可用格式，则设为空菜单。若菜单中的选项不符合clipcc可用格式，则将对应选项设为空。  