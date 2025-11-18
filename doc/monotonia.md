## Crecimiento y decrecimiento
  Si $f$ es una función derivable definida en un intervalo, entonces

  - $f$ es creciente si, y sólo si, la derivada es mayor o igual que cero;
  - $f$ es decreciente si, y sólo si, la derivada es menor o igual que cero; y
  - $f$ es constante si, y sólo si, la derivada es cero.
  
  Para estudiar el crecimiento de la función $f(x)=2x^3-3x^2-12x+1$, estudiamos el signo de la derivada. Primero vemos dónde se anula. 

::: {.sage}
<script type="text/x-sage">
    sage: f= 2*x^3-3*x^2-12*x+1
    sage: df = diff(f,x)
		sage: df

		sage: solve(df,x)
</script>
:::

$f'(x)=6x^2-6x-12=0$ si y sólo si $x\in\{-1,2\}$.  

Como sabemos donde se anula la derivada, también sabemos donde *no* se anula. Esto es, la función es monótona en $]-\infty,-1]$, en $[-1,2]$ y en $[2,+\infty[$. Evaluando la derivada en un punto de cada intervalo, terminamos:

  - $f'(-3)=60>0$, y por tanto $f$ es creciente $]-\infty,-1]$;
  
  - $f'(0)=-12<0$, en consecuencia $f$ es decreciente $[-1,2]$; y,
  
  - $f'(8)=324>0$, por lo que $f$ es creciente $[2,+\infty[$.
  

::: {.sage}
<script type="text/x-sage">
		sage: solve(df>0,x)
</script>
:::

¿Sabrías decir algo sobre los máximos y mínimos relativos de esta función?
  

  
