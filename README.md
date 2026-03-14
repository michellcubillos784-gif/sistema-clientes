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
git add clientes.txt inventario.txt
git commit -m "Agregar información inicial de clientes e inventario"
git push origin main

# Crear y cambiar a la rama
git checkout -b ventas

# Editar ventas.txt
echo "VentaID | Cliente | Producto
1 | Maria | Laptop" > ventas.txt

git checkout main
git merge ventas
git push origin main

# Commit en la rama
git add ventas.txt
git commit -m "Registrar primera venta"

# Subir rama a GitHub
git push origin ventas
