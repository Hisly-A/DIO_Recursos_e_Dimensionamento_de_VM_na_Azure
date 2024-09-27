# DIO - Recursos e Dimensionamento de VM na Azure
Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure


## Criação de uma máquina virtual na Azure

Abra o portal da [`Azure`](https://portal.azure.com), clique em **Máquinas virtuais** no menu lateral do portal



Clique em **+ Criar** e clique na opção **Máquina virtual do Azure**.



Na próxima tela preencha os campos necesários nos grupos **Detalhes do projeto** e **Detalhes da instância**.



No campo **Opções de disponibilidade** do grupo **Detalhes da instância** selecione a opção **Nenhuma redundância infraestrutura necessária**, mas não deixe de reparar nas demias opções:



Selecionando a opção *Conjunto de dimensionamento de máquinas virtuais* repare na mensagem de aviso:



Essa opção é ideal para empresas que precisam de aumento da capacidade das máquinas virtuais de forma automática, por exemplo em época de Black Friday.

No campo **Conjunto de dimensionamento de máquinas virtuais** clique em **Criar novo** e **OK** para abrir a tela de configuração e visualizar as opções disponíveis:



Repare na descrição das opções *Flexível* e *Uniforme*:



No campo **Contagem de instâncias** é definido o número de máquinas virtuais que devem aumentar por vez:



Clique no link **Configurar opções de escala** e veja as opções disponíveis:



No campo **Política de redução horizontal** repare nas opções:


Avançando, repare nas opções de **Modo de dimensionamento**:


Ao clicar em **Dimensionamento automático**, clique no link **Configurar** da caixa de texto que se abriu:



Clique no símbolo de lápis e veja as demais opções:



Voltando à página inicial da configuração, no campo **Zona de disponibilidade** é possível selecionar mais de uma zona, sendo que cada uma corresponde à um datacenter:



Preencha os demais campos necessários:



Repare na descrição do campo **Executar com descontro de Spot do Azure**, sendo essa opção geralmente utilizada em máquinas virtuais destinadas ao desenvolvimento ou teste:



No campo **Tamanho**, clique em **Ver todos os tamanhos**.



Na tabela que se abre repare nas opções disponíveis de tamnhos de VM e suas descrições:



No campo **Selecione as portas de entrada** vem selecionada por padrão a opção *RDP (3389)*, sendo necessário alterar para portas mais seguras: 



Após finalizar o preenchimento das informações nesta primeira tela, clique em **Avançar: Discos**:



Nesta etapa repare nas opções disponíveis no campo **Tipo de disco de SO**:



Lembre-se de marcar a opção **Excluir com VM**, para que o disco criado seja excluído juntamente com a máquina virtual quando esta não for mais necessária, e assim evitar cobranças desnecessárias na fatura.



Também é possível *Criar e anexar um novo disco* ou *Anexar um disco existente* caso queira adicionar um disco de outra unidade descontinuada:


Após finalizar o preenchimento das informações nesta tela, clique em **Avançar: Rede**:




## Links utilizados

- https://azure.microsoft.com/en-us/explore/global-infrastructure/geographies/

- https://portal.azure.com/
  
