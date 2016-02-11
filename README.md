DrillDownTool - profiling/investigating/analysing various subsystems like NFS, SMB/CIFS, ISCSI based on IOPS, throughput and latency.

This tool is intended for Solaris based OSs like Illumos. It has Dtrace as backend.

Overview of this tool:

ISCSI                                NFS                       CIFS
|                                    |                         |
|                                    |                         |
-->IOPS                              -->IOPS                   -->IOPS
      |                                    |                         |
      -->VOLUME                            -->FS                     -->FS
	      |                                |                         |
	      -->IP                            -->IP                     -->IP
      -->IP                                -->IP                     -->IP
    	  |                                    |                         |
    	  -->VOLUME                            -->FS                     -->FS