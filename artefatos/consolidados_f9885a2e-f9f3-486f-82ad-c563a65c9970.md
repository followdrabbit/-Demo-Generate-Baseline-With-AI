```markdown
<ul>
  <li><strong>Nombre del Control:</strong> Desactivar access control lists (ACLs)</li>
  <li><strong>ID del Control:</strong> AWS.Storage.Amazon S3.Static.2024.0001</li>
  <li><strong>Justificación:</strong> La desactivación de ACLs permite que el control de acceso se gestione exclusivamente a través de políticas de gestión de acceso, simplificando la administración y auditoría de permisos.</li>
  <li><strong>Riesgos Mitigados:</strong> Reducción de configuraciones complejas que pueden llevar a brechas de seguridad debidas al manejo incorrecto de ACLs.</li>
  <li><strong>Criticidad:</strong> Alta, debido a que las ACLs pueden introducir errores en la gestión de permisos.</li>
  <li><strong>Referencias:</strong> <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html">Best practices for securing your account and data in Amazon S3</a></li>
</ul>

<ul>
  <li><strong>Nombre del Control:</strong> Asegurar que los bucket policies no permitan acceso público</li>
  <li><strong>ID del Control:</strong> AWS.Storage.Amazon S3.Static.2024.0002</li>
  <li><strong>Justificación:</strong> Prevenir el acceso no autorizado a los datos almacenados en Amazon S3.</li>
  <li><strong>Riesgos Mitigados:</strong> Acceso público no intencionado que podría llevar a la exposición de datos sensibles.</li>
  <li><strong>Criticidad:</strong> Alta, dado que el acceso público a datos puede derivar en incidentes de seguridad importantes.</li>
  <li><strong>Referencias:</strong> <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html">Identity and Access Management for Amazon S3</a>, <a href="https://docs.aws.amazon.com/awssupport/latest/user/getting-started.html#trusted-advisor">AWS Trusted Advisor</a></li>
</ul>

<ul>
  <li><strong>Nombre del Control:</strong> Implementar el principio de mínimo privilegio</li>
  <li><strong>ID del Control:</strong> AWS.Storage.Amazon S3.Static.2024.0003</li>
  <li><strong>Justificación:</strong> Limitar permisos a solo lo necesario para reducir riesgos de cambios accidentales o intencionados de configuración.</li>
  <li><strong>Riesgos Mitigados:</strong> Minimiza el impacto de cuentas o usuarios comprometidos al limitar el alcance de sus permisos.</li>
  <li><strong>Criticidad:</strong> Alta, dado que el exceso de permisos puede resultar en acceso no autorizado a los datos.</li>
  <li><strong>Referencias:</strong> <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-iam.html">Identity and Access Management for Amazon S3</a></li>
</ul>

<ul>
  <li><strong>Nombre del Control:</strong> Usar roles de IAM para aplicaciones y servicios que requieren acceso a Amazon S3</li>
  <li><strong>ID del Control:</strong> AWS.Storage.Amazon S3.Static.2024.0004</li>
  <li><strong>Justificación:</strong> Evita el uso de credenciales permanentes, que pueden ser difíciles de rotar y manejar.</li>
  <li><strong>Riesgos Mitigados:</strong> El uso de credenciales a largo plazo puede llevar a riesgos de seguridad si son comprometidos.</li>
  <li><strong>Criticidad:</strong> Alta, las credenciales comprometidas pueden llevar a accesos no autorizados.</li>
  <li><strong>Referencias:</strong> <a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html">IAM Roles</a></li>
</ul>

<ul>
  <li><strong>Nombre del Control:</strong> Considerar el cifrado de datos en reposo</li>
  <li><strong>ID del Control:</strong> AWS.Storage.Amazon S3.Static.2024.0005</li>
  <li><strong>Justificación:</strong> Protege los datos de accesos no autorizados mientras están almacenados.</li>
  <li><strong>Riesgos Mitigados:</strong> Exposición de datos debido a acceso físico a los discos de almacenamiento en AWS.</li>
  <li><strong>Criticidad:</strong> Alta, el cifrado es fundamental para proteger los datos en caso de compromisos a nivel de infraestructura.</li>
  <li><strong>Referencias:</strong> <a href="https://docs.aws.amazon.com/AmazonS3/latest/userguide/serv-side-encryption.html">Protecting data with server-side encryption</a></li>
</ul>

<ul>
  <li><strong>Nombre del Control:</strong> Aplicar el cifrado de datos en tránsito</li>
  <li><strong>ID del Control:</strong> AWS.Storage.Amazon S3.Static.2024.0006</li>
  <li><strong>Justificación:</strong> Protege los datos desde y hacia S3 durante la transferencia en la red.</li>
  <li><strong>Riesgos Mitigados:</strong> Interceptación de datos en tránsito por parte de atacantes.</li>
  <li><strong>Criticidad:</strong> Alta, dado que los datos en tránsito son vulnerables a ataques del tipo man-in-the-middle.</li>
  <li><strong>Referencias:</strong> <a href="https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-ssl-requests-only.html">s3-bucket-ssl-requests-only</a></li>
</ul>
```
