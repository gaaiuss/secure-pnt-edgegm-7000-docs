### Web GUI Configuration

Configuração via web GUI.

---

#### PTP Configuration

1. GNSS funcionando:
   - Conectar a antena na entrada correta GNSS. No painel deve aparecer o LED
     correspondente ao GNSS/GPS. O reconhecimento pode demorar.

     ![Front Panel Overview](img/front_panel_overview.png)

2. Clock source OK:
   - Em Clock Central configurations, habilitar o GNSS e outras fontes de clock
     em Sync source, após isso, deverá aparecer como PRS (Primary reference source) o GNSS.

     ![Clock Central Configuration](img/clock_central_config.png)

   - Também é possível definir manualmente qual fonte será primária ou secundária
     pelo dropdown ao lado da fonte.

     ![Clock Central Configuration](img/clock_central_config2.png)

3. IP/VLAN OK:
   - Configuration -> System -> IP: Checar/adicionar os IPs das interfaces
     (VLANs) que serão usadas pelo PTP.

     ![IP Configuration](img/ip_config.png)

   - Configuration -> Advanced -> L2 & Switching-> VLANs -> Configuration:
     Adicionar a "Allowed VLANs" a VLAN criada utilizando uma vírgula e definir
     qual porta utilizará a respectiva VLAN.

     ![Global VLAN Config](img/global_vlan_config.png)

4. PTP Clock habilitado:
   - Em PTP clock configuration, adicionar as instâncias de 0 a 3.
   - Configurar o domínio PTP em HW Domain.
   - Definir qual o profile a ser utilizado para cada instância.

     ![PTP Clock Config](img/ptp_clock_config.png)

5. Configurar portas PTP:
   - Dentro da instância, configurar as portas que serão usadas no PTP.

     ![PTP Instance](img/ptp_instance.png)

   - Marcar a porta a ser utilizada, habilitar o protocolo que será utilizado
     pelo clock, associar a VLAN em questão e clicar em "Apply".

     ![PTP Instance](img/ptp_instance2.png)

---
