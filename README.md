# Updater Clover V2

<img src="assets/images/updater-clover-icon-official.png" alt="Updater Clover V2" width="96">

Aplicativo gratuito para macOS focado em manutenção do Clover com mais segurança e praticidade. O app ajuda a atualizar arquivos essenciais da EFI, criar backups completos, restaurar backups salvos e consultar informações do sistema em uma interface simples e bilíngue.

## Visão geral

O Updater Clover V2 foi criado para facilitar o fluxo de atualização e recuperação da partição EFI, especialmente em ambientes Hackintosh com Clover.

Com ele, você pode:

- atualizar arquivos essenciais do Clover na EFI selecionada
- criar backups completos automaticamente
- restaurar backups anteriores com poucos cliques
- visualizar informações detalhadas do sistema
- alternar entre português e inglês
- usar tema claro, escuro ou automático

## Funcionalidades

### Update Clover

- atualiza `EFI/BOOT/BOOTX64.efi`
- atualiza `EFI/CLOVER/CLOVERX64.efi`
- atualiza drivers UEFI essenciais
- suporta modo simples e modo completo
- no modo completo, também sincroniza `EFI/CLOVER/tools`

### Backup EFI

- cria backups completos da EFI
- salva os backups em `~/EFI_BACKUPS`
- lista os backups disponíveis
- abre a pasta de backups
- copia o caminho do backup

### Restore EFI

- restaura qualquer backup EFI válido para a partição selecionada
- ajuda a recuperar ambientes Clover com mais rapidez

### Info System

- exibe bootloader atual
- mostra partição EFI selecionada
- informa versão do macOS
- mostra CPU, GPU, memoria e discos
- permite gerar screenshot da tela de informacoes

### Extras

- interface bilíngue: `PT-BR` e `EN`
- temas `Light`, `Dark` e `Auto`
- botão `Open Sym` para abrir a pasta `sym` configurada

## Compatibilidade

- macOS Ventura
- macOS Tahoe

## Download

Baixe a release atual:

[Updater Clover V2.dmg](https://github.com/maxpicelli/Updater-Clover-v2/releases/download/1.0.0/Updater-Clover-V2.dmg)

## Site do projeto

[GitHub Pages](https://maxpicelli.github.io/Updater-Clover-v2/)

## Demo em video

- YouTube: [Updater Clover V2 Demo](https://youtu.be/4cEeanEK1qo)

## Prints

### Update Clover

![Update Clover Dark](assets/images/update-clover-dark.png)

![Clover Builder Dark](assets/images/clover-builder-dark.png)

![Clover Builder Light](assets/images/clover-builder-light.png)

### Backup EFI

![Backup EFI Dark](assets/images/efi-backup-dark.png)

![Backup EFI Light](assets/images/efi-backup-light.png)

### Info System

![Info System](assets/images/info-sistema.png)

## Observações

- algumas ações podem exigir senha de administrador para montar ou alterar a EFI
- antes de atualizar, confirme sempre a partição EFI selecionada
- manter backups em `~/EFI_BACKUPS` ajuda na recuperação rápida do sistema

## Apoio

Se o projeto te ajudar, você pode apoiar o desenvolvimento:

[Doar via PayPal](https://www.paypal.com/donate?business=picelli1974%40outlook.com&amount=4.99&currency_code=USD&item_name=Updater+Clover+V2+Donation)

## Agradecimentos

Agradecimento especial ao [@hnanoto](https://github.com/hnanoto) pelo projeto original que serviu como base e inspiração para esta evolução do aplicativo.

[Projeto original no GitHub](https://github.com/hnanoto/Update_Clover)
