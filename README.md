# tripwire

    ./deploy tripwire hostsfile /Users/christopher/Documents/DataNexus/Platform/Source/datanexus

To display the latest report:
     
    ./deploy tripwire hostsfile /Users/christopher/Documents/DataNexus/Platform/Source/datanexus
    

There will be a single error with the host database file:

    ./deploy tripwire ../confluent/hostsfile.none /Users/christopher/Documents/DataNexus/Platform/Source/datanexus check

Blindly accept the results by updating the database and run the check:

    ./deploy tripwire ../confluent/hostsfile.none /Users/christopher/Documents/DataNexus/Platform/Source/datanexus update
    ./deploy tripwire ../confluent/hostsfile.none /Users/christopher/Documents/DataNexus/Platform/Source/datanexus check
 
If you see an error related to the database backup, run the sequence again:

    ./deploy tripwire ../confluent/hostsfile.none /Users/christopher/Documents/DataNexus/Platform/Source/datanexus update
    ./deploy tripwire ../confluent/hostsfile.none /Users/christopher/Documents/DataNexus/Platform/Source/datanexus check
 