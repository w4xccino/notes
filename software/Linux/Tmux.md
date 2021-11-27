# Qué es Tmux?

[[Tmux]] es una aplicación que permite dividir terminales en una sola ventana. ES decir que se pueden correr varias operaciones simultaneamente en una sola terminal por medio de paneles y sesiones configurables. Todo eso se puede configurar, es genial pero no se como usarlo aún.

## Instrucciones básicas de Tmux.
Así como [[VIM]], [[Tmux]], también tiene se pueden establecer atajos de teclado personalizados. Y, en efecto, también se puede establecer  una tecla líder para hacer ello. Por defecto la combinación de teclas es `Ctrl+b`

### Sesiones
 - Crear una sesión: `tmux`
 - Crear sesion con nombre: `tmux new -s NOMBRE`
 - Entrar a la ultima sesion: `tmux a`
 - Entrar en una sesion por su nombre: `tmux a -t NOMBRE`
 - Borrar una sesion: `tmux kill-session -t NOMBRE`

### Ventanas
Las ventanas son como pestañas en cualquier navegador, se pueden recorrer con diferentes atajos de teclado.
- **Crear una nueva ventana**: `C`
- **Cerrar una ventana**: `&`
- **Ir a la ventana anterior**: `p`
- **Ir a la ventana siguiente**: `n`
- **Listar ventnas**: `w`

### Paneles
Son divisiones dentro de una ventana.
- **Crear nuevo panel horizontalmente**: `"`
- **Crear nuevo panel verticalmente** : `%`
- **Moverse**: `flechitas de teclado`
- **Cerrar panel**: `x`
- **Convertir un panel en ventana**: `!`
