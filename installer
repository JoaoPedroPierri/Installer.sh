#!/bin/env bash

# Limpar console

clear

# Title

echo '

██████╗  █████╗  ██████╗███╗   ███╗ █████╗ ███╗   ██╗

██╔══██╗██╔══██╗██╔════╝████╗ ████║██╔══██╗████╗  ██║

██████╔╝███████║██║     ██╔████╔██║███████║██╔██╗ ██║

██╔═══╝ ██╔══██║██║     ██║╚██╔╝██║██╔══██║██║╚██╗██║

██║     ██║  ██║╚██████╗██║ ╚═╝ ██║██║  ██║██║ ╚████║

╚═╝     ╚═╝  ╚═╝ ╚═════╝╚═╝     ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝' |lolcat

echo

while true; do

  

  # Menu

  echo

  echo 'Escolha uma das opções abaixo:'|lolcat

  echo

  echo '1 - Instalar Pacotes'|lolcat

  echo '2 - Proucurar por pacotes'|lolcat

  echo '3 - Apagar pacotes' |lolcat

  echo '4 - Informações do pacote' |lolcat

  echo '5 - Pacote instalado' |lolcat

  echo '6 - Sair do programa' | lolcat

  echo

  read ALT

  echo

  # Condições

  if [ $ALT == '1' ];then

    echo 'Digite o nome do pacote que queira instalar:'

    echo

    read PACKAGE_NAME

    echo

    echo 'Digite sua senha sudo se pedir...'

    echo

    sudo pacman -S $PACKAGE_NAME

    echo

    echo 'Pacote instalado com sucesso...'

    echo

  fi

  if [ $ALT == '2' ];then

    echo 'Digite o nome do pacote que está procurando:'

    echo

    read PACKAGE_SEARCH

    echo

    pacman -Ss $PACKAGE_SEARCH

    echo

  fi

  if [ $ALT == '3' ];then

    echo 'Digite o nome do pacote que deseja apagar (LEMBRE-SE QUE VAI APAGAR AS CONFIGURAÇÕE DO PACOTE TAMBÉM)'

    echo

    read PACKAGE_DELETE

    echo

    echo 'Digite a senha sudo se pedir...'

    echo

    sudo pacman -Rns $PACKAGE_DELETE

    echo

    echo 'Pacote deletado com sucesso...'

    echo

  fi

  if [ $ALT == '4' ];then

    echo 'Digite o nome do pacote que deseja se informar:'

    echo

    read PACKAGE_INFORMATION

    echo

    pacman -Qi $PACKAGE_INFORMATION

    echo

  fi

  if [ $ALT == '5' ];then

    echo 'Digite o nome do pacote para saber se está instalado na maquina (Se aparecer é por que está instalado)'

    echo

    read PACKAGE_INSTALL

    echo

    pacman -Qs $PACKAGE_INSTALL

    echo

  fi

  if [ $ALT == '6' ];then

    echo 'Deseja sair s/n?'

    read OPC

    echo

    if [ $OPC == 's' ];then

      echo 'Saindo...'

      exit 0

    else

      continue

    fi

  fi

done
