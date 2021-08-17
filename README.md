# Pytorch-tutorial
## Tensor Attributes
```
torch.dtype
torch.device
torch.layout #存储方式
```
### Creating Tensors Using Data

基于构造器实现（将tensor类型改为默认的float32） 
torch.Tensor(data) 

基于工厂模式实现（tensor类型为原始data的类型）
```
> torch.get_default_dtype()
torch.float32
```
torch.tensor(data)
torch.as_tensor(data)
torch.from_numpy(data)
```
> o1 = torch.Tensor(data)
> o2 = torch.tensor(data)
> o3 = torch.as_tensor(data)
> o4 = torch.from_numpy(data)

> print(o1)
> print(o2)
> print(o3)
> print(o4)
tensor([1., 2., 3.])
tensor([1, 2, 3], dtype=torch.int32)
tensor([1, 2, 3], dtype=torch.int32)
tensor([1, 2, 3], dtype=torch.int32)
```
![](https://github.com/sdx19961008/Pytorch-tutorial/blob/main/tensor.png)

### Creation Options Without Data
```
> print(torch.zeros([2,2]))
tensor([
    [0., 0.],
    [0., 0.]
])

> print(torch.ones([2,2]))
tensor([
    [1., 1.],
    [1., 1.]
])

> print(torch.rand([2,2]))
tensor([
    [0.0465, 0.4557],
    [0.6596, 0.0941]
])
```
