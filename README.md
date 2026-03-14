# sistema-clientes
# Crear carpeta local
mkdir sistema-clientes
cd sistema-clientes

# Inicializar repositorio
git init

# Crear archivos
touch clientes.txt ventas.txt inventario.txt

# Primer commit
git add .
git commit -m "Primer commit: estructura inicial del proyecto"

# Conectar con GitHub (usa la URL que te da GitHub)
git remote add origin https://github.com/tu_usuario/sistema-clientes.git

# Subir cambios
git push -u origin main
