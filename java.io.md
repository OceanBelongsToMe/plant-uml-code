```plantUML
@startuml
package java.io <<Frame>> {
	class InputStream << (A,orchid) >> {
		{abstract} +void read() throws IOException
		+int read(byte[] input) throws IOException
		+int read(byte[] input, int offset, int length) throws IOException
		+long skip(long n) throws IOException
		+long available() throws IOException
		+void close() throws IOException
		.. uncommonly used ..
		+void mark(int readAheardLimit)
		+void reset() throws IOException
		+boolean markSupported()
	}
	class OutputStream << (A,orchid) >> {
		{abstract} +void wirte(int b) throws IOException
		+void wirte(byte[] data) throws IOException
		+void wirte(byte[] data, int offset, int length) throws IOException
		+void flush() throws IOException
		+void close() throws IOException
	}
}
@enduml
```