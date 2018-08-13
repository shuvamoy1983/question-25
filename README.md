# question-25

abstract class vehicle{
}


class autonomouscar extends vehicle {
}

abstract class parkingLot {
 parkingLot(int slotNumber) {
        isOccupied = false;
        this.slotNumber = slotNumber;    
    }
   
    boolean isOccupied() {
        return isOccupied;
    }
    
    int getSlotNumber() {
        return slotNumber;
    }
     
    void park() {
        isOccupied = true;
    } 
     
    void unPark() {
       isOccupied = false;
    }
    
}

class AutonomousCarSlot extends parkingLot {
 
    AutonomousCarSlot(int slotNumber)  {
        super(slotNumber);
    } 
}
