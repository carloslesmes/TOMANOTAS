# Toma de notas

$$
GM = \left(\prod_{i=1}^{n} x_i\right)^{1/n}
$$

For two numbers $a$ and $b$:

$$
GM = \sqrt{ab}
$$

```julia
function geometric_mean(x)
    return exp(sum(log, x) / length(x))
end

values = [2, 8, 32]
println(geometric_mean(values))
```
