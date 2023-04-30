Download Link: https://assignmentchef.com/product/solved-csce438-hw-5
<br>
<ol>

 <li><em>[50 points (0.65pt each)] </em>Choose the statements below that are <strong>TRUE</strong>:

  <ul>

   <li>Strict, Sequential and Causal Consistencies are Data-Centric consistency models.</li>

   <li>Eventual Consistency, Monotonic Reads and Monotonic Writes are Client-Centricconsistency models.</li>

   <li>Strict Consistency assumes absolute global time.</li>

   <li>In Strict Consistency a “read is expected to return the value resulting from themost recent write”</li>

   <li>Strict Consistency can be achieved if we have GPS.</li>

   <li>In Sequential Consistency “the result of any execution is the same as if the (readand write) operations by all processes on the data were executed in an arbitrary order.”</li>

   <li>In Causal Consistency, if an update U1 causes another update U2 to occur, then,U1 should be executed before U2 at each copy.</li>

   <li>Causal Consistency is stronger than sequential consistency.</li>

   <li>In Eventual Consistency, if no updates take place for a long time, all replicas willgradually become consistent.</li>

   <li>In a Monotonic Read, “if a process reads the value of a data item x, then anysuccessive read operation on x by that process will always return that same value or a more recent value.”</li>

   <li>In a Write Monotonic consistent store, a write operation by a process on a dataitem x is completed before any successive write operation on x by the same process.</li>

   <li>One implementation of Sequential Consistency is to use a centralized process,called sequencer.</li>

   <li>Write-through will impact caching in a distributed file system.</li>

   <li>The read-ahead in distributed file systems, requests chunks of data when they areneeded.</li>

   <li>The first version of NFS ran over UDP, using Sun RPC.</li>

   <li>NFS uses caching at the client (caching data, file attributes and pathname bindings).</li>

   <li>All NFS writes are write-through to disk.</li>

   <li>Inconsistencies between local caches and server in NFS are solved by comparingtime-stamps.</li>

   <li>NFS always invalidated data after some time (3 seconds for data in open files).</li>

   <li>NFS version 2 extends the client-side buffer caching to disk, in 64KB chunks.</li>

   <li>NFS version 3 continued to use UDP, because its simplicity.</li>

   <li>NFS version 3 started to support 64bit file sizes.</li>

   <li>GFS was designed with Google’s application workload specifically in mind.</li>

   <li>In GFS, during a write operation, the master for a chunk sends data to replicasin a daisy chain.</li>

   <li>In GFS, if the master reboots and then finds a chunck server has a newer versionnumber for a chunk, it adopts that version number.</li>

   <li>In GFS, if a chunk server dies, then the master decrements the count of replicasfor all chunks on that chunk server.</li>

   <li>GFS was designed for small streaming reads.</li>

   <li>GFS was designed for large sequential writes that append.</li>

   <li>In GFS, the performance of operations is very good for all apps.</li>

   <li>GFS architecture contains one master server.</li>

   <li>In the GFS architecture there is one chunk server for each chunk.</li>

   <li>The master server in GFS holds metadata and most frequently accessed data files.</li>

   <li>The master server in GFS holds all metadata in RAM.</li>

   <li>A read/write operation with a chunk server in GFS specifies the chunk handleand the byte range.</li>

   <li>In GFS, the client issues control/metadata requests to the chunk servers.</li>

   <li>A client in GFS uses no caching.</li>

   <li>The GFS consistency model defines “consistent” as: file region all clients see assame, regardless of replicas they read from.”</li>

   <li>In GFS, the serial success result of a write operation is DEFINED.</li>

   <li>In GFS, a successful record append data mutation is DEFINED.</li>

   <li>In GFS, a successful concurrent write is CONSISTENT but DEFINED.</li>

   <li>In GFS, a failure of a write or record append operation is INCONSISTENT.</li>

   <li>BigTable is a sparse, centralized persistent multi-dimensional sorted map.</li>

   <li>The map in BigTable is indexed by row key, column key and timestamp.</li>

   <li>A row range (partition) in BigTable is also called tablet.</li>

   <li>The items in a BigTable cell are stored in decreasing timestamp order.</li>

   <li>BigTable is an alternate way for storing data than GFS and it implements its ownreplication.</li>

   <li>BigTable processes share the same machines with MapReduce and GFS machines.</li>

   <li>In the BigTable, there is a master server and many tablet servers.</li>

   <li>In the BigTable, a client communicates directly with tablet servers for reads/writes.</li>

   <li>The master server in BigTable maintains the set of live tablet servers and thecurrent assignment of tablets to tablet servers.</li>

   <li>The memtable is an in RAM storage for storing the committed writes that arrivedat a tablet server.</li>

   <li>When memtable size increases and reaches a threshold, it is frozen and committedto an SSTable in GFS.</li>

   <li>The execution of a MapReduce program creates a Master process and severalWorker processes.</li>

   <li>The master process of a MapReduce program assigns map and reduce tasks toworker processes.</li>

   <li>The intermediate results of a MapReduce program are stored in GFS.</li>

   <li>If the master process of a MapReduce program crashes a new master is electedthrough Chubby.</li>

   <li>A Partition Function in a MapReduce program is used for ensuring that recordswith the same intermediate key end up at the same worker.</li>

   <li>A MapReduce program will use information from GFS (location of replicas) todecide which file blocks will be processed by which worker process.</li>

   <li>When a worker process in MapReduce segfaults, the information about the recordit processed is lost.</li>

   <li>If the master process in MapReduce sees two failures for the same record, then ittells the next worker to skip the record.</li>

   <li>In HDFS, a DataNode is the same as a ChunkServer in GFS.</li>

   <li>In HDFS, a NameNode is the same as the Master Node in GFS.</li>

   <li>A block in GFS is the same as a chunk in HDFS.</li>

   <li>If a system can provide strong consistency, the programming model (how theprogrammer uses the API) is greatly simplified.</li>

   <li>A Mobile Cloud consists of Distributed Storage and Distributed Data Processing</li>

   <li>A k-out-of-n system is an n-component system that works if and only if k or lesscomponents work</li>

   <li>Radio transmission is one of the major source of energy consumption on mobiledevices.</li>

   <li>In “Resource allocation For edge computing” lecture data is allocated in a waythat the overall data retrieval energy is minimized.</li>

   <li>In “Resource allocation For edge computing” lecture, the failure probability estimation includes failures due to disconnection from network.</li>

   <li>In “Resource allocation For edge computing” lecture, Importance Sampling wasused for approximating the expected distance between two nodes.</li>

   <li>The Read-ahead (prefetch) policy in a distributed file system, minimizes the waitwhen it actually is needed.</li>

   <li>The Write-on-close policy in a distributed file system is synonym with sessionsemantics.</li>

   <li>The VFS layer in NFS stands for Vectored File System.</li>

   <li>In MapReduce, the arguments for a mapping function is a key and a value.</li>

   <li>In MapReduce, the arguments for a mapping function is a key and a value.</li>

   <li>The Partition Function in MapReduce ensures that records with the same intermediate key end up at the same worked.</li>

  </ul></li>

</ol>