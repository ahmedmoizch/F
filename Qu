class queue{
    int max = 5;
    int queue[] = new int[max];
    int size;
    int front;
    int rear;

    public void enqueue(int data){
        queue[rear] = data;
        rear = (rear+1)%max;
        size = size+1;
    }
    public void insertF(int data){
        front = (front - 1 + max) % max;
        queue[front] = data;
        size++;
    }

    public void insertR(int data){
        queue[rear] = data;
        rear = (rear + 1) % max;
        size++;
    }

    public int dequeue(){
        int data = queue[front];
        front = (front + 1)%max;
        size = size-1;
        return data;
    }

    public void deleterear(){
        rear = (rear-1+max) % max;
        size--;
    }

    public void show(){
        for(int i=0;i<size;i++){
            System.out.print(queue[(i+front)%max] + " ");
        }
    }
}

public class ps{
    public static void main(String[] args) {
        queue p = new queue();
        p.enqueue(5);
        p.show();
        p.insertF(4);
        p.insertR(6);
        p.deleterear();
        p.show();

    }
}
