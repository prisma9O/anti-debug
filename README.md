# anti-debug
anti-debug checks (Android)

Notas:
- El código ha sido desarrollado C++ aunque seria fácil adaptarlo a C. He ido bastante justo de tiempo.
- No me ha dado tiempo a implementar las syscalls para las diferentes arquitecturas
- El check de integridad es muy simple y solo funciona en arquitectura x86
- No me ha dado tiempo a implementar funciones anti-tracing como la inserción de breakpoints


Caraterísticas:
- Incluye un check que verifica el fichero /proc/self/status/
- Incluye un check de integridad que tiene como objetivo detectar software breakpoints
- Incluye un check que verifica la presencia de depuradores JDWP
- Mide el tiempo de ejecución como medida anti-tracing
