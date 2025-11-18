## Convexidad y concavidad 
En esta sección estudiamos la curvatura de una función dos veces derivable.

::: {.callout-note}
Para poder calcular la curvatura de una función, es necesario que sea dos veces derivable en un dominio.
:::


::: {.callout-tipe}
1. Si $f''$ es positva, entonces $f$ es convexa.
2. Si $f''$ es negativa, entonces $f$ es cóncava.
:::


::: {.sage}
<script type="text/x-sage">
ddf=diff(df,x)
ddf
</script>
:::

::: {.sage}
<script type="text/x-sage">
    if ddf > 0: 
        print("La función es convexa")
    else:
        print("La función es cóncava")
</script>
:::


Como $f''(x)=6x+6$, tenemos:
1. En $]-\infty,-1)$ la función es cóncava
2. En $(-1,\infty)$ la función es convexa 

