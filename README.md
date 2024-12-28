# surveillance dns

## Description

Cette vue personnalisée surveille les événements du serveur DNS et du client sur Windows Server. Il fournit un aperçu des opérations critiques, des erreurs, des avertissements et des journaux d'informations liés au service DNS.

## niveaux surveillés
- Critical (1)
- Error (2)
- Warning (3)
- Information (4)

## sources d'evenements incluses
- DNS-Server-Service: For server-side DNS operations.
- DNS Client Events: For client-side DNS events.

## identifiants d'evenment surveillés
- **2**: DNS Server startup.
- **4**: DNS Server shutdown.
- **409**: Name resolution failure.
- **501-502**: Zone loading failures.
- **6001-6002**: DNS replication issues.

## comment utiliser
1. Import the XML file into the Event Viewer on a Windows Server.
2. Monitor DNS events through the `DNS Service Monitoring` custom view.

## Installation
- Download `dns_service_monitoring.xml`.
- Open Event Viewer > Custom Views > Import Custom View > Select the XML file.
