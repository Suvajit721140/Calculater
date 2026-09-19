class SequenceWorker extends Thread {

    private String workerid;

    public SequenceWorker(String id) {
        this.workerid = id;
    }

    @Override
    public void run() {
        try {
            for (int i = 1; i <= 3; i++) {
                System.out.println(
                    "Worker thread [" + workerid + "] tracking step " + i
                );

                Thread.sleep(500);
            }
        } catch (InterruptedException e) {
            System.out.println("Exception Interrupted");
        }
    }
}

public class ThreadExtensionDemo {

    public static void main(String[] args) {

        SequenceWorker t1 = new SequenceWorker("Alpha");
        SequenceWorker t2 = new SequenceWorker("Beta");

        t1.start();
        t2.start();
    }
}
