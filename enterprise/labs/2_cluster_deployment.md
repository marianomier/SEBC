```
{
  "timestamp" : "2017-11-30T20:29:16.406Z",
  "clusters" : [ {
    "name" : "Mariano",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "4207935488"
          }, {
            "name" : "hive_metastore_server_max_message_size",
            "value" : "420793548"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_enable_impersonation",
            "value" : "false"
          }, {
            "name" : "hiveserver2_java_heapsize",
            "value" : "4207935488"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "2324928921"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "391"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-63-6.ec2.internal"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "hive_proxy_user_groups_list",
          "value" : "hue,hive,sentry"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "sentry_service",
          "value" : "sentry"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-0b80585cbff36f28a424590b34ef8439",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-4a27045cacedefb1e3b821ccc980b857",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-7401753d3f4191ef185385a048114ad0",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "6776688c-f4c0-42f5-936e-25103ed45947"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-4a27045cacedefb1e3b821ccc980b857",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bxmsafpwsw2e4hhniog0jpr5g"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-4a27045cacedefb1e3b821ccc980b857",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9jduk8ven8sj43mw62is6bxsi"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "enableSecurity",
          "value" : "true"
        } ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-4a27045cacedefb1e3b821ccc980b857",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8liwrccispftclg4bt5vjhfjt"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-56e09c7561f786985632f7cf23660679",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5bnjgkchanuljhassurxklaqu"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-7401753d3f4191ef185385a048114ad0",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "6776688c-f4c0-42f5-936e-25103ed45947"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4lm9lbsog8vq7bkqk5offttzb"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-63-6.ec2.internal"
        }, {
          "name" : "database_password",
          "value" : "hue_password"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_sentry_safety_valve",
          "value" : ""
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-7401753d3f4191ef185385a048114ad0"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "sentry_service",
          "value" : "sentry"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-4a27045cacedefb1e3b821ccc980b857",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5a7z9h67y1rtkq0bencgtkpq2"
          }, {
            "name" : "secret_key",
            "value" : "Nztl0W2VqV4EJ95KwGfbv9CwoDWtIo"
          } ]
        }
      }, {
        "name" : "hue-KT_RENEWER-4a27045cacedefb1e3b821ccc980b857",
        "type" : "KT_RENEWER",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5h4crtmsc1yk9rvh32gir4uz5"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-63-6.ec2.internal:3306"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-7401753d3f4191ef185385a048114ad0",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "6776688c-f4c0-42f5-936e-25103ed45947"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2alwxijc4ggnsrkw0ij20z26p"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "12"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "1"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/data00/yarn/nm,/data01/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/data00/yarn/container-logs,/data01/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "6921"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "13577"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "6"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "80"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "XLpnQs2ZpRrdu53h9pOUAbJsaMwEYG"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-0b80585cbff36f28a424590b34ef8439",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9n34sktudcnydpfj6omc3ziav"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-0b80585cbff36f28a424590b34ef8439",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "94j23n95b2riwjqo9jy2lhk5m"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-4a27045cacedefb1e3b821ccc980b857",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c9mltfk35oz9qkcx0q7yyqbxw"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-7401753d3f4191ef185385a048114ad0",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "6776688c-f4c0-42f5-936e-25103ed45947"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "52cyrorv7o79s2nge40mdnwaz"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-0b80585cbff36f28a424590b34ef8439",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "46"
          }, {
            "name" : "role_jceks_password",
            "value" : "en6cos04ni7kgfcti8ggqpqrp"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/data00/dfs/dn,/data01/dfs/dn"
          }, {
            "name" : "dfs_datanode_data_dir_perm",
            "value" : "700"
          }, {
            "name" : "dfs_datanode_failed_volumes_tolerated",
            "value" : "1"
          }, {
            "name" : "dfs_datanode_http_port",
            "value" : "1006"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "dfs_datanode_port",
            "value" : "1004"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "400"
          }, {
            "name" : "rm_io_weight",
            "value" : "200"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/data00/dfs/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/data00/dfs/nn,/data01/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/data00/dfs/snn"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_encrypt_data_transfer_algorithm",
          "value" : "AES/CTR/NoPadding"
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "SIPSRoAg8QNd86vGk3uvcmZbesa6r6"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "hbHCWDKsDK4fxV3TDCm8mVdt67bQs7"
        }, {
          "name" : "hadoop_security_authentication",
          "value" : "kerberos"
        }, {
          "name" : "hadoop_security_authorization",
          "value" : "true"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "dQYZFQZc1RJbmxFGfikGjOOKeoJOjf"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "20"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-0b80585cbff36f28a424590b34ef8439",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-0b80585cbff36f28a424590b34ef8439",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dpdgcgdzdr9imban3i9u7pnov"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-4a27045cacedefb1e3b821ccc980b857",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7xatc3ibwp5dqskx0l7hk94eh"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-7401753d3f4191ef185385a048114ad0",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "6776688c-f4c0-42f5-936e-25103ed45947"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "673quwvwvgmnf0tbe0tgifsx9"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-0b80585cbff36f28a424590b34ef8439",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2yeckmje9fqmz4faqipkzvav2"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-4a27045cacedefb1e3b821ccc980b857",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b6859ktc9onuv2n5b9cqdbaax"
          } ]
        }
      }, {
        "name" : "hdfs-GATEWAY-56e09c7561f786985632f7cf23660679",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-HTTPFS-7401753d3f4191ef185385a048114ad0",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "6776688c-f4c0-42f5-936e-25103ed45947"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bvm98n73sncs4k518tb53xsce"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-0b80585cbff36f28a424590b34ef8439",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cz0a225xsaxo0gtoh2tym5r6n"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-56e09c7561f786985632f7cf23660679",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6qtim76busz2jz2zjgvu8319e"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-7401753d3f4191ef185385a048114ad0",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "6776688c-f4c0-42f5-936e-25103ed45947"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3cgbh4jrsaycm0sv94euw0za0"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-0b80585cbff36f28a424590b34ef8439",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "48"
          }, {
            "name" : "role_jceks_password",
            "value" : "aghl4il9h20m063l21q4iq01d"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-4a27045cacedefb1e3b821ccc980b857",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "a21o3vfayyx2h6de80l1cvxql"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    }, {
      "name" : "sentry",
      "type" : "SENTRY",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "sentry_server_database_host",
          "value" : "ip-172-31-63-6.ec2.internal"
        }, {
          "name" : "sentry_server_database_password",
          "value" : "sentry_password"
        }, {
          "name" : "sentry_service_admin_group",
          "value" : "hive,impala,hue,solr,kafka,chingon"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "sentry-GATEWAY-0b80585cbff36f28a424590b34ef8439",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-4a27045cacedefb1e3b821ccc980b857",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-7401753d3f4191ef185385a048114ad0",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "6776688c-f4c0-42f5-936e-25103ed45947"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-SENTRY_SERVER-56e09c7561f786985632f7cf23660679",
        "type" : "SENTRY_SERVER",
        "hostRef" : {
          "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "55r6xzinckl59c0nghhnrx40p"
          } ]
        }
      } ],
      "displayName" : "Sentry"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "8b95db3d-c4fe-471b-b8a3-111e8d0a3396",
    "ipAddress" : "172.31.48.156",
    "hostname" : "ip-172-31-48-156.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "f50a4ce1-6da5-45be-b548-66f65895863f",
    "ipAddress" : "172.31.55.238",
    "hostname" : "ip-172-31-55-238.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "6776688c-f4c0-42f5-936e-25103ed45947",
    "ipAddress" : "172.31.60.84",
    "hostname" : "ip-172-31-60-84.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8",
    "ipAddress" : "172.31.63.6",
    "hostname" : "ip-172-31-63-6.ec2.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-56e09c7561f786985632f7cf23660679",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "92cd4962c292dc4f018bbfc986841137852cab1518c7434c1c237ed7a989facc",
    "pwSalt" : 2678223150900317591,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-56e09c7561f786985632f7cf23660679",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "5504e502b8b29ca54c933b478e04e1b9c54d8ea0c24c9eafff786bb45c2fe45f",
    "pwSalt" : 6467562908599503836,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-56e09c7561f786985632f7cf23660679",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "225bec13120a83129525de08719496bb6dec692f268f59e8f1fb1abb94f617df",
    "pwSalt" : -7565461385853428228,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-56e09c7561f786985632f7cf23660679",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "6928db4c88d89a6b13f38ade5ee82fab7138f3874610a587c4a909498a3d89d9",
    "pwSalt" : 3783333549640394181,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "b2300033d1be78690ab6b067d8d20ffa5c4d066a152089c454e7181242a79d94",
    "pwSalt" : -962749756476861982,
    "pwLogin" : true
  }, {
    "name" : "marianomier",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "8db291e6bb88124883e96e85471be4c71730754c868dfa05c7eb9bf6350b2b27",
    "pwSalt" : -6375340840619249593,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "53224195519230342adee5c6acfc3a8903edeb1783cfbc193fcbb3ec44204833",
    "pwSalt" : 7742472073223866358,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.10.2",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170626-1942",
    "gitHash" : "15f547c8802e02d59901ee3fe1c5c5733eab0227",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-63-6.ec2.internal:3306"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-56e09c7561f786985632f7cf23660679",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "27mxz535bo9zjvmeroc0r0uti"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-56e09c7561f786985632f7cf23660679",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "v3953a2aijtf29x46pzuavqj"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-56e09c7561f786985632f7cf23660679",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "cethiqxehdejh9ncmbctvrbh7"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-56e09c7561f786985632f7cf23660679",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "57cv0u1a8xlm9i42mr99406q0"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-56e09c7561f786985632f7cf23660679",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "618661d9-89c8-4665-a8b3-9d2500d108b8"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "5had9mz2z39r7uugh1apht4l9"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "AD_USE_SIMPLE_AUTH",
      "value" : "false"
    }, {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/28/2012 1:10"
    }, {
      "name" : "KDC_ADMIN_PASSWORD",
      "value" : "BQIAAAA+AAEAC01BUklBTk8uQ09NAAxjbG91ZGVyYS1zY20AAAABWh8GHgEAFwAQt4ZJ0d4CngQDRlqMXfageAAAAAE="
    }, {
      "name" : "KDC_ADMIN_USER",
      "value" : "cloudera-scm@MARIANO.COM"
    }, {
      "name" : "KDC_HOST",
      "value" : "ip-172-31-63-6.ec2.internal"
    }, {
      "name" : "KRB_ENC_TYPES",
      "value" : "arcfour-hmac"
    }, {
      "name" : "KRB_MANAGE_KRB5_CONF",
      "value" : "true"
    }, {
      "name" : "MAX_RENEW_LIFE",
      "value" : "604800"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    }, {
      "name" : "SECURITY_REALM",
      "value" : "MARIANO.COM"
    } 
    ``
    }}
