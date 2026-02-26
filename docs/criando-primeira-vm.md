
# Criando sua Primeira VM na Azure (2026)

## Introdução

Este guia fornece um passo a passo para criar uma máquina virtual na plataforma Microsoft Azure. São apenas 10 passos até sua primeira VM!

## Pré-requisitos

- Conta ativa na Azure
- Acesso ao Portal Azure
- Permissões suficientes para criar recursos

## Sumário
1. [Passos para Criar uma VM](https://github.com/amandioca/nts-dio-microsoft-azure-essentials/edit/primeira-vm/docs/criando-primeira-vm.md#passos-para-criar-uma-vm)
2. [Próximos Passos](https://github.com/amandioca/nts-dio-microsoft-azure-essentials/edit/primeira-vm/docs/criando-primeira-vm.md#pr%C3%B3ximos-passos)
3. [Ao terminar, exclua!](https://github.com/amandioca/nts-dio-microsoft-azure-essentials/edit/primeira-vm/docs/criando-primeira-vm.md#ao-terminar-exclua)
4. [Referências](https://github.com/amandioca/nts-dio-microsoft-azure-essentials/edit/primeira-vm/docs/criando-primeira-vm.md#refer%C3%AAncias)

## Passos para Criar uma VM

1. Navegue para [portal.azure.com](https://portal.azure.com) e faça login com suas credenciais

2. Digite `máquinas virtuais` na barra de pesquisa

3. Em **Serviços**, selecione a opção **Máquinas virtuais**

4. Na página "*Infraestrutura de computação | Máquinas virtuais*", clique em **Criar** e selecione **Máquina virtual**

5. Em **Detalhes da instância**:
    * Escolha o **Nome da máquina virtual** da sua preferência (Sugestão `myFirstVM`)
    * Em **Imagem**, selecione _Windows Server 2025 Datacenter: Azure Edition - x64 Gen 2_

> Se você optar por selecionar "Executar com desconto de Spot do Azure", terá desconto na VM, porém disponibilidade limitada. Selecione (i) para mais detalhes.

![alt text](./imgs/criando-primeira-vm/image.png)

6. Selecione o **Tamanho** da sua máquina.

      O tamanho escolhido determina fatores como capacidade de processamento, memória e capacidade de armazenamento.
      As **opções disponíveis e valores podem variar** de acordo com a **Zona de disponibilidade** escolhida.

![alt text](./imgs/criando-primeira-vm/image3.png)

7. Em **Conta de administrador**, forneça um usuário como `azureuser` e uma senha, conforme o requisito de complexidade definido.

![alt text](./imgs/criando-primeira-vm/image2.png)

8. Em **Regras de porta de entrada**, escolha **Permitir portas selecionadas** e, em seguida, selecione RDP (3389) e HTTP (80) na lista suspensa.

![alt text](./imgs/criando-primeira-vm/image4.png)

9. Deixe os padrões restantes e clique em **Revisar + criar**

10. Após passar na validação, você terá o resumo da sua VM e valor/hora total. Clique em criar.

![alt text](./imgs/criando-primeira-vm/image5.png)

## Próximos Passos

Após criar a VM, você pode:

- Conectar via RDP (Windows) ou SSH (Linux)
- Instalar aplicações necessárias
- Configurar backups
- Monitorar performance

![alt text](./imgs/criando-primeira-vm/image6.png)

## Ao terminar, exclua!

Para para zerar o custo e não consumir seus créditos ou gerar gastos, exclua sua VM e recursos associados ao fim do laboratório. 
Também é possível apenas desligar, mas é possível que ainda assim haja gastos com recursos associados como armazenamento e IP público. 

![alt text](./imgs/criando-primeira-vm/image7.png)

> Na página inicial você pode acompanhar seus créditos disponíveis.

## Referências
- [Início Rápido: Criar uma máquina virtual do Windows no Portal do Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)
- [Portal Azure](https://portal.azure.com)
