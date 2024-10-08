# Listar interfaces e visualizar suas descrições

```
display interface description
```
![image](https://github.com/user-attachments/assets/3948a189-6684-4fc5-b3b6-6960cf82834a)

- *VLANIF* normalmente relacionado a MPLS.

![image](https://github.com/user-attachments/assets/53a228d8-9c2e-4e00-9769-8bca6d744359)

- *XGigabitEthernet 0/0/18* Interface fisica do equipamento, fibras conectada diretamente.

# Verificar sinal da interface/fibra

```
display transceiver diagnosis interface XGigabitEthernet 0/0/18
```
![image](https://github.com/user-attachments/assets/e638ecd9-3fcc-48d7-83d3-e6742a68e2c2)

- Verificar o campo ( RxPower(dBm)    -6.40  ), EX.: Sinal tá sendo -6.40dBm.
- Campo (Low Alarm Threshold)          -26.02, É o limite de sinal maximo que pode chegar.

# Verificar status da interface
```
display interface XGigabitEthernet 0/0/1
```
-*Last physical down time* mostra o horario da queda.

![image](https://github.com/user-attachments/assets/92caf266-c5aa-4cda-99e0-7f1e564a63ef)


# Verificar modelo de gbic

- Transceiver Type               :10GBASE_LR_SFP (Verificar capacidade do GBIC)
- Wavelength(nm)                 :1270           (Verificar frequencia)
- Transfer Distance(m)           :80000(9um)     (Verificar quantos GBIC)

![image](https://github.com/user-attachments/assets/96da0c40-735e-4b1d-b0d1-10fdaea530a7)




Verificação de Interface "Down" em um Switch
*Confirmar Status da Interface*: Use o comando para checar se a interface está "down" (ex: display interface description x ).

*Verificar o Sinal da Interface*: Analise o nível de sinal recebido para verificar se há problemas físicos ou falhas no cabo (ex: display transceiver diagnosis interface XGigabitEthernet 0/0/18 ).

Registrar o Horário da Queda: Consulte os logs para identificar o momento exato em que a interface caiu (ex:  display interface XGigabitEthernet 0/0/18 ).

Monitorar o Sinal Máximo Recebido: Verifique se houve flutuações no sinal antes da queda, o que pode indicar problemas com o cabo ou equipamento (ex: zabbix e grafana).


