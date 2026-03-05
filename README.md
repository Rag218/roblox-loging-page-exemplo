 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index af62858885b0017562c6618aa3ecb9cd41e575e6..175319a55f689e51f2ddaa1140b4738674b437a9 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,29 @@
-# roblox-loging-page-exemplo
\ No newline at end of file
+# Simulação de Login (Local)
+
+Este projeto fornece uma página HTML de login no repositório (`public/index.html`) e um servidor Node local para simular o recebimento das credenciais.
+
+> Importante: é uma simulação genérica e educativa, sem copiar marca real.
+
+## Como executar
+
+```bash
+npm start
+```
+
+Abra `http://localhost:3000` no navegador.
+
+## Como testar
+
+```bash
+npm test
+```
+
+O teste sobe o servidor, envia credenciais de exemplo e valida o retorno da API e os logs no terminal.
+
+## O que acontece ao enviar
+
+Ao enviar o formulário:
+- o frontend manda JSON para `POST /login`
+- o backend imprime no terminal:
+  - usuário informado
+  - senha informada
 
EOF
)
