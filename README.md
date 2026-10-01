# ValeFlow

Sistema web para gestão e conciliação de Vale-Transporte, desenvolvido para centralizar a importação, processamento, conferência e tratamento de dados de VT.

## 🚀 Sobre o projeto

O ValeFlow foi desenvolvido para simplificar o trabalho operacional de gestão de Vale-Transporte, reduzindo erros de cálculo, duplicidades, cobranças indevidas e inconsistências nos dados importados.

O sistema trabalha com o ciclo completo da competência:

**Importação → Processamento → Validação → Exceções → Correções → Conferência → Finalização**

## ⚙️ Funcionalidades

- 🔐 Autenticação por e-mail corporativo
- 📊 Dashboard da competência ativa
- 📅 Gestão de competências
- 📥 Importação de arquivos `.xlsx`, `.xls`, `.csv` e `.txt`
- 🔍 Validação e pré-visualização dos dados importados
- 💰 Gestão de tarifas e valores diários
- 🧮 Cálculo automático do Vale-Transporte
- ⚠️ Gestão e tratamento de exceções
- 🗑️ Exclusão e limpeza de dados de teste
- 📈 Histórico e acompanhamento das competências

## 🛠️ Tecnologias

- React
- TypeScript
- Tailwind CSS
- Supabase
- Vite
- PapaParse
- XLSX

## 📐 Regra de cálculo

O cálculo do Vale-Transporte segue:

```text
Dias Ativos = Dias Úteis - (Férias + Afastamentos)

Tarifa Diária = Tarifa por Trecho × Trechos Diários

Valor Calculado = Dias Ativos × Tarifa Diária
