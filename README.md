# CloudFormation

## Arquitectura

1. **VPC (Red Privada Virtual)**
   - Aisla la infraestructura en una red segura
  

2. **Subnets**
   - Distribuidas en múltiples zonas de disponibilidad (AZ) para alta disponibilidad.
   - Configuradas para soportar tanto tráfico de red
  
3. **Instancias EC2 (5 Servidores)**
   - 5 instancias distribuidas en diferentes subnets para distribuir la carga.

4. **Load Balancer (ELB)**
   - Balancea automáticamente el tráfico entre las 5 instancias EC2.
   - Configurado con políticas para manejar picos de tráfico y garantizar disponibilidad.
  
5. **Internet Gateway (IGW)**
   - Permite a las instancias en subnets públicas acceder a Internet.
