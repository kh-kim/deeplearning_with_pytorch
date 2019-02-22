# Adam Optimizer

## Learning Rate 튜닝

### LR이 너무 클 떄

### LR이 너무 작을 때

## Adam (Adaptive Moment Estimation)

```py
optim = torch.optim.Adam(model.parameters())
```

```py
loss.backward()
optim.step()
```