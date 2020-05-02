# Tv.java
public class Tv{
	private int length;//长度
	private int width;//宽度
	private int height;//高度
	private int psb;//电源板
	private String turnon;//打开
	private int watch;//观看
	private String turnoff;//关闭
	public Tv() {
	this.length=80;
	this.width=60;
	this.height=40;
	this.psb=5;
	this.turnon="on";
	this.watch=8;
	this.turnoff="off";
	}
	public Tv(int length,int width, int height, int psb, String turnon,int watch,String turnoff) {
		super();
		this.length = length;
		this.width = width;
		this.height = height;
		this.psb = psb;
		this.turnon =turnon;
		this.watch = watch;
		this.turnoff =turnoff;
		}
	public int getLength() {
		return length;
		}
	public void setLength(int length) {
		this.length = length;
		}
	public int getWidth() {
		return width;
		}
	public void setWidth(int width) {
		this.width = width;
		}
	public int getHeight() {
		return height;
		}
	public void setHeight(int height) {
		this.height = height;
		}
	public int getPsb() {
		return psb;
		}
	public void setPsb(int psb) {
		this.psb = psb;
		}
	public String getTurnon() {
		return turnon;
		}
	public void setTurnon(String turnon) {
		this.turnon = turnon;
		}
	public int getWatch() {
		return watch;
		}
	public void setWatch(int watch) {
		this.watch = watch;
		}
	public String getTurnoff() {
		return turnoff;
		}
	public void setTurnoff(String turnoff) {
		this.turnoff = turnoff;
		}
	public void Neibu() {
		System.out.println("电视长为"+length+"cm,宽为"+width+"cm,高为"+height+"cm,电源板有"+psb+"个.");
		}
	public void Waibu() {
		System.out.println("按"+turnon+"打开电视，正在观看第"+watch+"频道，按"+turnoff+"关掉电视.");
	}
	public static void main(String[] args) {
		Tv c=new Tv(80,60,40,5,"on",8,"off");
		c.Neibu();
		c.Waibu();
	}
}
