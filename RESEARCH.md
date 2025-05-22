# RESEARCH.md

## ¿Qué son los componentes de React y cómo se reutilizan?

Los **componentes** en React son bloques reutilizables de código que representan partes de una interfaz de usuario. Pueden ser **funciones** o **clases** que devuelven elementos JSX. Los componentes permiten dividir la UI en piezas pequeñas y manejables, cada una con su propia lógica y estilo. Se reutilizan al importar y renderizar el mismo componente en diferentes partes de la aplicación, lo que evita la duplicación de código. También se pueden **parametrizar usando props**, lo que permite mostrar información diferente usando el mismo componente base. Esto mejora la **mantenibilidad** y **escalabilidad** de las aplicaciones React.

---

## ¿Qué es el "lifting state up" y cuándo deberías usarlo?

El _"lifting state up"_ es una técnica en React que consiste en **mover el estado compartido** entre varios componentes hijos hacia su **componente padre común**. Esto permite que el componente padre controle el estado y lo pase a los hijos mediante **props**. Se utiliza cuando múltiples componentes necesitan acceder o modificar el mismo estado para mantenerse sincronizados. Por ejemplo, si dos componentes deben responder a una misma acción del usuario, es mejor que el estado se gestione en un nivel superior. Esto ayuda a mantener una **única fuente de verdad** y a evitar inconsistencias. Es una práctica recomendada para gestionar estados compartidos de forma más **clara** y **estructurada**.
