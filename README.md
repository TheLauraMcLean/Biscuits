public class Biscuits {

    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);

        int Biscuitpacket;

        int Biscuitbox;

        int Leftoverpackets;

        int Leftoverbiscuits;

        System.out.print("Enter the number of biscuits:");
        int Biscuitcount = scan.nextInt();

        Biscuitpacket = (Biscuitcount / 12);
        Biscuitbox = (Biscuitpacket / 30);
        Leftoverpackets = Biscuitpacket - Biscuitbox * 30;
        Leftoverbiscuits = Biscuitcount - (Biscuitpacket * 12);

        if (Biscuitpacket == 0) {
            System.out.print(" There are no packets of biscuits: ");
        } else if (Biscuitpacket == 1) {
            System.out.print(" There is " + Biscuitpacket + " packet of biscuits: ");
        } else {
                System.out.print(" There are " + Biscuitpacket + " packets of biscuits: ");
        }

        if (Biscuitbox == 0) {
            System.out.print("no boxes with ");
        } else if (Biscuitbox == 1) {
            System.out.print(Biscuitbox + " box with ");
        } else {
                System.out.print(Biscuitbox + " boxes with ");
        }

        if (Leftoverpackets == 0) {
            System.out.print("no leftover packets and ");
        } else if (Leftoverpackets == 1) {
            System.out.print(Leftoverpackets + " leftover packet and ");
        } else {
                System.out.print(Leftoverpackets + " leftover packets and ");
        }

        if (Leftoverbiscuits == 0) {
            System.out.print("no leftover biscuits");
        } else if (Leftoverbiscuits == 1) {
            System.out.print(Leftoverbiscuits + " leftover biscuit");
        } else {
                System.out.print(Leftoverbiscuits + " leftover biscuits");
        }
    }
}
