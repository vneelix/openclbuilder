# openclbuilder
Simple OpenCL program builder for C.
CL Builder use support structure
```C
typedef struct	s_cl_builder {
	cl_platform_id		platform;
	cl_device_id		device;
	cl_context		context;
	cl_command_queue	queue;
	cl_program		program;
}				t_cl_builder;
```
Signature is
```C
openclbuilder(t_cl_builder *cl, char *src_dir, char *inc_dir)
```
You can create a temporary cl_builder structure, pass a directory with source code files and a directory with header files (optional). CL Builder compiles each file separately taking into account the header files and then link the binary file
