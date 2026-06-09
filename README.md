# 🏭 Dona Rita Embalagens · Sistema de Controle de Não Conformidades

Sistema web completo para registro, acompanhamento e gestão de **Não Conformidades (NCs)** na produção de embalagens.

---

## 🚀 Funcionalidades

- ✅ **Dashboard** com gráficos em tempo real (Chart.js)
- ✅ **CRUD completo** de não conformidades (produto, palete, motivo, quantidade, ação, fotos)
- ✅ **Fotos** (até 5 por NC, com compressão automática)
- ✅ **Cronômetros ao vivo** para NCs abertas (dias, horas, minutos, segundos)
- ✅ **QR Code** individual por NC com **modo visitante somente leitura**
- ✅ **Impressão** de relatório da NC com QR Code incluso
- ✅ **Histórico** de todas as alterações de cada NC
- ✅ **Controle de usuários** com dois níveis:
  - **Admin** (`qualidade / 1304`) – acesso total, gerencia usuários, exclui NCs
  - **Padrão** (`operador / 1234`) – cria/edita NCs, sem permissão de excluir
- ✅ **Filtros** por status, palete e busca textual
- ✅ **Responsivo** (desktop e mobile)
- ✅ **Armazenamento offline** via `localStorage` (dados salvos no navegador)
- ✅ **Firebase Config** incluso e preparado para futura migração para Firestore

---

## 🔐 Acessos Padrão

| Usuário     | Senha | Tipo  | Permissões                          |
|-------------|-------|-------|-------------------------------------|
| `qualidade` | 1304  | Admin | Total (CRUD, usuários, excluir NCs) |
| `operador`  | 1234  | Padrão| Criar, editar, resolver, reabrir    |

> ⚠️ **Altere as senhas** após o primeiro acesso na seção "Usuários" (visível apenas para admin).

---

## 📱 Modo Visitante (QR Code)

Cada NC possui um **QR Code** que, ao ser escaneado, abre uma página **somente leitura** com todos os detalhes da NC.  
**Nenhuma alteração é permitida** nesse modo.

Exemplo de URL gerada: