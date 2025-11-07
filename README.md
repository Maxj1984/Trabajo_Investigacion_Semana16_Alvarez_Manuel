Paquete de prácticas para MSYS2+MinGW (CLion)
Contenido: 3 proyectos
01_ast_only       - Construcción y despliegue de AST (Árbol de Sintaxis Abstracta) de expresiones aritméticas
02_ast_to_tac     - Genera código de tres direcciones (TAC) a partir del AST
03_tac_opt_codegen- Genera TAC, aplica optimizaciones simples (constant folding, DCE) y genera código C
Instrucciones rápidas:
  - Instala MSYS2 y paquetes: mingw-w64-x86_64-gcc mingw-w64-x86_64-cmake mingw-w64-x86_64-make mingw-w64-x86_64-bison mingw-w64-x86_64-flex
  - En MSYS2 MinGW64 shell:
      cd /path/to/compilers_practicas_msys2/<project> (el path va a cambiar dependiendo de cual proyecto se va a ejecutar)
      mkdir build && cd build (este comando es para linux, si estas en windows ejecuta cada uno por separado ya que && no es reconocido en el cmd)
      cmake -G "MinGW Makefiles" ..
      mingw32-make
      ./<executable> "a * (b + 3)"
