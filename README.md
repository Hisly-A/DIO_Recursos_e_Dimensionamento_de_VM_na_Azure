# DIO - Recursos e Dimensionamento de VM na Azure
Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure


## Criação de uma máquina virtual na Azure

Abra o portal da [`Azure`](https://portal.azure.com), clique em **Máquinas virtuais** no menu lateral do portal

![AZ05-01](https://github.com/user-attachments/assets/6d4e554c-7c0b-4050-b2fd-234dc67bf3ad)

Clique em **+ Criar** e clique na opção **Máquina virtual do Azure**.

![AZ05-02](https://github.com/user-attachments/assets/b813a241-0aec-459a-aae9-fccd8e9b2bc4)

Na próxima tela preencha os campos necessários nos grupos **Detalhes do projeto** e **Detalhes da instância**.

![AZ05-03](https://github.com/user-attachments/assets/4efa6c82-472e-442b-aa42-e65ba086b21b)

No campo **Opções de disponibilidade** do grupo **Detalhes da instância** selecione a opção **Nenhuma redundância infraestrutura necessária**, mas não deixe de reparar nas demais opções:

![AZ05-04](https://github.com/user-attachments/assets/7275afde-14ed-4ebb-a38d-73a55a124441)

Selecionando a opção *Conjunto de dimensionamento de máquinas virtuais* repare na mensagem de aviso:

![AZ05-06](https://github.com/user-attachments/assets/2756939c-5ccf-4742-9e1b-9efc273c0157)

Essa opção é ideal para empresas que precisam de aumento da capacidade das máquinas virtuais de forma automática, por exemplo em época de Black Friday.

No campo **Conjunto de dimensionamento de máquinas virtuais** clique em **Criar novo** e **OK** para abrir a tela de configuração e visualizar as opções disponíveis:

![AZ05-07](https://github.com/user-attachments/assets/0cbf4b41-a8a9-4888-b438-b774976f6788)

Repare na descrição das opções *Flexível* e *Uniforme*:

![AZ05-08](https://github.com/user-attachments/assets/fcd8bea2-815a-493c-96d1-9aa4dc957953)

No campo **Contagem de instâncias** é definido o número de instâncias de máquinas virtuais que devem aumentar por vez:

![AZ05-09](https://github.com/user-attachments/assets/a73caaa7-b344-4fe3-808d-154bfbc81004)

Clique no link **Configurar opções de escala** e veja as opções disponíveis:

![AZ05-10](https://github.com/user-attachments/assets/f9cd60fd-de40-49cd-9cc4-71a8c039caa6)

No campo **Política de redução horizontal** repare nas opções:

![AZ05-11](https://github.com/user-attachments/assets/75f7119a-243f-4bc0-8f7b-09819e1faf2b)

Avançando, repare nas opções de **Modo de dimensionamento**:

![AZ05-12](https://github.com/user-attachments/assets/a13460df-c6cf-48b8-a3f7-c1da45be6db3)

Ao clicar em **Dimensionamento automático**, clique no link **Configurar** da caixa de texto que se abriu:

![AZ05-13](https://github.com/user-attachments/assets/3355c853-87a0-4214-838d-85140ac7e5a4)

Clique no símbolo de lápis e veja as demais opções:

![AZ05-14](https://github.com/user-attachments/assets/b08d94e7-9aa6-4e81-875a-0e9cd3130238)

![AZ05-15](https://github.com/user-attachments/assets/1eca24d6-7652-4909-9c3b-ad2a3cf187ee)

![AZ05-16](https://github.com/user-attachments/assets/0b495290-ba28-48d4-a979-78f9a26b6848)

![AZ05-17](https://github.com/user-attachments/assets/b417cf38-9548-4317-87d2-29198687e39d)

![AZ05-18](https://github.com/user-attachments/assets/93f0e6fb-deb9-4f9e-b4aa-c03357756d18)

Voltando à página inicial da configuração, no campo **Zona de disponibilidade** é possível selecionar mais de uma zona, sendo que cada uma corresponde à um datacenter:

![AZ05-05](https://github.com/user-attachments/assets/d5524ea5-d2b9-478a-a5ce-62a18cf1588f)

Preencha os demais campos necessários:

![AZ05-19](https://github.com/user-attachments/assets/b10543b3-6e23-442d-8ce2-bb2ce4f43fd0)

![AZ05-20](https://github.com/user-attachments/assets/a7d822b7-e046-443f-8ee0-34266d6f3061)

Repare na descrição do campo **Executar com descontro de Spot do Azure**, sendo essa opção geralmente utilizada em máquinas virtuais destinadas ao desenvolvimento ou teste e nunca de produção:

![AZ05-21](https://github.com/user-attachments/assets/403ec087-0927-4eac-8703-0cdad323cae2)

No campo **Tamanho**, clique em **Ver todos os tamanhos**.

![AZ05-22](https://github.com/user-attachments/assets/57a9ed63-4c66-4484-bc08-20d5bd8a0bd3)

Na tabela que se abre repare nas opções disponíveis de tamanhos de VM e suas descrições:

![AZ05-23](https://github.com/user-attachments/assets/bd5da21a-33e3-4d8c-b2dd-0800c8617746)

![AZ05-24](https://github.com/user-attachments/assets/8fe08a95-2794-4578-a61b-a6c060da909f)

No campo **Selecione as portas de entrada** vem selecionada por padrão a opção *RDP (3389)*, sendo necessário alterar para portas mais seguras: 

![AZ05-25](https://github.com/user-attachments/assets/e6777fed-8891-442b-90f6-ab22651ee8a3)

Após finalizar o preenchimento das informações nesta primeira tela, clique em **Avançar: Discos**:

![AZ05-26](https://github.com/user-attachments/assets/0c37e1e9-33a1-4911-a452-f81c4a362143)

Nesta etapa repare nas opções disponíveis no campo **Tipo de disco de SO**:

![AZ05-27](https://github.com/user-attachments/assets/2d6db361-5cb2-4335-b88e-d1ae994713b1)

![AZ05-28](https://github.com/user-attachments/assets/32459210-88f9-470a-9528-a5b5d9ea34be)

Lembre-se de marcar a opção **Excluir com VM**, para que o disco criado seja excluído juntamente com a máquina virtual quando esta não for mais necessária, e assim evitar cobranças desnecessárias na fatura.

![AZ05-29](https://github.com/user-attachments/assets/3ab1d96a-5a03-48bc-848a-c8292d3d24a8)

Também é possível *Criar e anexar um novo disco* ou *Anexar um disco existente* caso queira adicionar um disco de outra unidade descontinuada:

![AZ05-30](https://github.com/user-attachments/assets/54e7ba01-41a0-4d98-a30d-171064717b2b)

Após finalizar o preenchimento das informações nesta tela, clique em **Avançar: Rede**:

![AZ05-31](https://github.com/user-attachments/assets/fe843ce1-159b-46a3-b964-36948326dab0)

Preecha os campos necessários para a configuração de rede da máquina virtual:

![AZ05-32](https://github.com/user-attachments/assets/69f37fbe-1ca1-443e-9c90-1c690b89a3c6)

![AZ05-33](https://github.com/user-attachments/assets/618a9cbd-8baf-4cea-b25d-598d22381025)

Repare na observação do campo **Selecione as portas de entrada** devido ao uso da porta RDP (3389):

![AZ05-34](https://github.com/user-attachments/assets/81648e40-92e8-422b-8c53-057b141eb2b6)

Lembre-se de marcar o campo **Excluir o IP público e a NIC quando a VM for excluída** para evitar gastos desnecessários:

![AZ05-35](https://github.com/user-attachments/assets/136a2661-c0f3-4964-af40-88a80cf8cc6d)

Após clique em **Avançar: Gerenciamento**:

![AZ05-36](https://github.com/user-attachments/assets/e333c0a4-df87-4c29-9ba3-4c2d4d01dc94)

Preencha as opções de gerenciamento conforme sua necessidade:

![AZ05-37](https://github.com/user-attachments/assets/f55ee79b-240b-4efe-8613-f5e504f38fc6)

![AZ05-38](https://github.com/user-attachments/assets/1ef366f9-4026-4271-97ee-7219ae74d077)

Marque a opção **Habilitar backup** caso deseje que sejam feitos backups da máquina virtual:

![AZ05-39](https://github.com/user-attachments/assets/649c99e5-f428-421e-a878-2d7d1614644d)

Após clique em **Avançar: Monitoramento**:

![AZ05-40](https://github.com/user-attachments/assets/e757e349-76bc-4620-889c-5ff202e3d23d)

Ao clicar em **Habilitar regras de alerta recomendadas** é aberto um menu lateral para escolher as opções:

![AZ05-41](https://github.com/user-attachments/assets/1fd183a2-74e2-44ef-adfc-00c8783f083d)

![AZ05-42](https://github.com/user-attachments/assets/7f50fb3a-a05b-45b1-afbb-3e1b5c48e4a7)

Em **Diagnóstico** marque a opção **Desabilitar**, para não consumir memória, e após clique em **Avançar: Avançado**:

![AZ05-43](https://github.com/user-attachments/assets/5af9d0ed-bf26-47cb-9152-762c9c1754dc)

Clique na opção **Selecionar uma extensão para instalar** e verifique as extensões disponíveis:

![AZ05-44](https://github.com/user-attachments/assets/b946ce23-01b7-48ef-b3be-712002b68fe8)

![AZ05-45](https://github.com/user-attachments/assets/22d38a10-2fb6-4852-862d-ffcc963e5781)

Verifique os demais campos na aba **Avançado** e clique em **Avançar: Marcas**:

![AZ05-46](https://github.com/user-attachments/assets/faae7e44-0e28-47eb-88d8-92382d7f1785)

Na aba **Marcas** crie as tags necessárias e clique em **Avançar: Revisar + criar**:

![AZ05-47](https://github.com/user-attachments/assets/c9b3af03-1212-470e-9c97-d102f2f2140a)

Na aba **Revisar + criar** repare que é apresentada uma prévia do valor a ser pago, e clique em **Criar**:

![AZ05-48](https://github.com/user-attachments/assets/f9d923f6-41cb-49f1-a72b-3ae67af9a565)


## Criação de um pool de hosts ou imagem

Vá para a **Área de Trabalho Virtual do Azure** e clique em **Criar um pool de hosts**:

![AZ05-49](https://github.com/user-attachments/assets/f403f3e0-e667-4602-b88f-44a363537ea6)

Repare que no campo **Tipo de pool de hosts** há as opções *Pessoal* e *Em pool*. A opção *Pessoal* é indicada quando é necessário criar uma sessão para um único usuário executar um software específico que somente ele irá utilizar, por exemplo.

![AZ05-50](https://github.com/user-attachments/assets/b5b65105-6226-4cef-90af-efdba1f1c564)

Preencha os demais campos e clique em **Próximo: Máquinas Virtuais**:

![AZ05-51](https://github.com/user-attachments/assets/5d7a40b7-bac4-4e33-b55c-8ca8db308472)

Realize o preenchimento das demais etapas e prossiga até chegar na aba **Examinar + criar** e clique em **Criar**:

![AZ05-52](https://github.com/user-attachments/assets/00feceee-b55f-45f1-897d-0694db2cc310)


## Links utilizados

- https://portal.azure.com/
  
