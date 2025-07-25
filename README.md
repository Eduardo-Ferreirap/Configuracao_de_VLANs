# Projeto de Configuração de VLANs com Cisco Packet Tracer

> **Autor:** Eduardo Ferreira de Paula  
> 📧 ferreira.eduardop30@gmail.com  
> 🌐 [LinkedIn](https://linkedin.com/in/eduardo-ferreira-de-paula1)  

## 📘 Descrição

Este projeto consiste na criação de uma rede segmentada com **VLANs** (Virtual LANs), simulada no **Cisco Packet Tracer**, com o objetivo de isolar o tráfego de diferentes grupos de usuários: `Alunos`, `Funcionários` e `Convidados`. A rede foi configurada utilizando **3 switches Layer 2 (L2)** e segue os princípios fundamentais do curso técnico em Redes e os conceitos da certificação **Cisco CCNA**.

## 🎯 Objetivos

- Configurar dispositivos básicos (nome, senha, banner, etc.)
- Criar e atribuir VLANs específicas para diferentes grupos
- Configurar interfaces de acesso e trunk
- Verificar o isolamento entre VLANs
- Validar comunicação entre hosts da mesma VLAN

## 🗺️ Topologia

A rede segue um modelo simples de campus com os seguintes elementos:

### 📌 VLANs

| VLAN | Nome         | Sub-rede          | Hosts             |
|------|--------------|-------------------|-------------------|
| 10   | ALUNOS       | 192.168.10.0/24   | PC aluno1, aluno2 |
| 20   | FUNCIONARIOS | 192.168.11.0/24   | PC func1, func2   |
| 30   | CONVIDADOS   | 192.168.12.0/24   | PC conv1, conv2   |

### 🔌 Equipamentos

- 3 Switches L2
- 6 PCs (2 por VLAN)
- Cabos Ethernet diretos e crossover
- Interfaces configuradas como **access** e **trunk**

## ⚙️ Configurações Importantes

- Senhas e acesso remoto configurados para simulação
- VLANs criadas com `name` correspondente ao grupo
- Criptografia de senhas habilitada (`service password-encryption`)
- Links trunk configurados com protocolo 802.1Q
- Interfaces access associadas corretamente às VLANs

⚠ **Nota:** As senhas usadas neste projeto (ex: `cisco`) são apenas para demonstração em ambiente de laboratório.

## ✅ Testes Realizados

### 🔄 Comunicação entre hosts da mesma VLAN
✅ Comunicação bem-sucedida entre dispositivos da mesma VLAN, inclusive em switches diferentes.

### 🚫 Isolamento entre VLANs diferentes
✅ Comunicação **bloqueada** entre dispositivos de VLANs distintas, validando o isolamento esperado com switches L2 (sem roteamento inter-VLAN).



# OBSERVAÇÃO
Documentação e arquivo .pkt estão disponíveis para Download neste repositório
