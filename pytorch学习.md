# 关于pytorch的使用
## 建立和访问张量
- 使用python列表初始化一个张量 example:
   x= torch.tensor() 使用具体“坐标”访问张量中的某个数据
  同样的，对于特殊的矩阵，可以使用一些特殊的函数来创建
  一些有用的函数可以访问某个张量的参数
  如x.dim  x.shape  在pytorch官网查询会很方便 
- 关于访问张量中的数据
   pytorch允许访问张量的切片
## 对张量的形状进行重塑
- flatten(拉平为张量) 对于张量x x.view(-1)
- make_row_vec(制作行向量) x.view(1,-1）
- 关于view函数的使用： https://pytorch.org/docs/stable/generated/torch.Tensor.view.html.
## 关于索引张量
- 整数索引张量 可以通过整数列表来完成对张量中数据的不同组合
  idx = [0, 1, 2]
  print('\nGet the diagonal:')
  print(a[idx, idx]) 通过这种方式修改或访问张量的对角线元素是被允许的
- torcg.arange函数
