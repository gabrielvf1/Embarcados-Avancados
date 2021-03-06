#  👁 Entrega 2

!!! success
    Revisado 2020-2

O que deve ser entregue?

- **Pasta:** `Entrega_2_FPGA_NIOS`
- **Vídeo** do projeto funcionando com uma explicação (aprox 1.5 min)

Nessa entrega iremos ter a mesma funcionalidade que a [Entrega 1](/Entrega1/) porém com o motor sendo acionado pelo NIOS (soft processor).

Para isso será necessário modificar o projeto criado no tutorial para possuir ao menos mais um periférico PIO (que será responsável por ler os botões). Além de adicionar esse novo periférico, nessa entrega iremos aprimorar nosso sistema com:

- Periférico JTAG deve gerar interrupção
- Periférico PIO que lida com o botão deve gerar interrupção
- Memória de programa separada da de dados

Uma vez que o JTAG começa a gerar interrupções não será mais necessário usar o *small driver* do JTAG, lembre de alterar isso no **bsp**. 

Comece por ler os botões sem interrupção, uma vez que estiver funcionando, utilize os sites a seguir como referência para implementar interrupção no NIOS:

Dicas:

- http://www.johnloomis.org/NiosII/interrupts/interrupt/interrupt.html
- https://www.altera.com/en_US/pdfs/literature/hb/nios2/n2sw_nii52006.pdf

## Rubrica

(incremental)

- A 
    - Insira um RTOS no NIOS para fazer o controle da aplicação, **ou**
    - Curva de aceleração no motor
- B
    - Implementar `VEL` no SWx
- C
    - Memória de dados separada da de programa
    - JTAG gerando interrupção.
    - PIO dedicado a ler botões (SWx) e controlar `EN` e `DIR`
    - Interrupção na leitura do botão
- D 
    - Entregou somente tutorial
- I
    - Não entregou nada
