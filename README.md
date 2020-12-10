# pick_meshs_gitee

## 运行说明

- 需要安装cuda10(低版本的不知道行不行,只在cuda10.1和10.2上试过,9.0以上应该都可以)

- 将以前的liboptix_prime.so.6.5.0 文件挪到`usr/lib`文件夹下

- 运行`./pick_meshs `  测试：`./pick_meshs -i a.glb -o out.glb`


## 输入说明

./pick_meshs [options]

  -h  | --help	帮助信息

  -i  | --infile <model_file_address(string)>	输入文件的地址 必要参数

  -o  | --outfile <model_file_address(string)>	输出文件的地址 必要参数

   -r  | --ray_number <sphere_vertex_number(int)> 射线产生球体的层级数量 非必要参数 
   
   -p  | --pick_flag <pick_flag(int)> 是否拾取模型 非必要参数(0为不拾取，1为拾取  默认为1)

## 注意事项

- 当原始文件中有多个buffer，导出后会变为一个buffer
