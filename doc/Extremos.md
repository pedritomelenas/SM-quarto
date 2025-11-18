## Extremos relativos

::: {.callout-tip title="Teoría básica"}
El cálculo de los máximos y mínimos relativos de una función $f$ se suele hacer en dos pasos.

1. En primer lugar se calculan los puntos críticos, es decir, resolvemos la ecuación $f'(x)=0$

1. Evaluamos la segunda derivada en los puntos críticos:

* si $f'(a)=0$, y además $f''(a)>0$, entonces $f$ tiene un mínimo relativo en $a$;
* si $f'(a)=0$, y además $f''(a)<0$, entonces $f$ tiene un máximo relativo en $a$.
:::

Si analizamos el signo de la derivada segunda de la función del ejemplo anterior en los puntos críticos que habíamos obtenido, concluimos cuál es mínimo y cuál es máximo.


::: {.sage}
<script type="text/x-sage">
ddf=diff(df,x)
ddf
</script>
:::

::: {.sage}
<script type="text/x-sage">
[ddf.subs({x:-1}), ddf.subs({x:2})]
</script>
:::


Como $f''(x)=12x-6$, tenemos:

* $f''(-1)=-18<0$, por tanto en $x=-1$ tenemos un máximo relativo;
* $f''(2)=18>0$, por tanto en $x=2$ tenemos un mínimo relativo.

::: {.callout-caution collapse="true"}
¿Concuerdan estas conclusiones con las que has obtenido estudiando el cambio de monotonía en torno a ambos puntos?
:::

::: {.callout-note collapse="true"}
Supongamos que queremos encontrar los extremos relativos de $f(x) = 2x^3-3x^2-12x+1$

Primero derivamos la funcion: $f'(x) = 6x^2-6x-12$

A continuación, buscamos los puntos críticos, es decir, los valores de x para los que $f'(x) = 0$

$f'(x) = 0 \;\Leftrightarrow\; x \in \{-1, 2\}$

Para ver si son máximo o mínimo, evaluamos en la segunda derivada: $f''(x) = 12x-6$
$f''(-1) = -6 < 0$, luego es máximo.
$f''(2) = 18 > 0$, luego es mínimo.
:::