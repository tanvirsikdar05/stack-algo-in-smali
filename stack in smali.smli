.class public LStack;
.super Ljava/lang/Object;

.field private size:I
.field private data:[Ljava/lang/Object;

.method public constructor <init>()V
    .registers 3

    const/4 v0, 10
    new-array v1, v0, [Ljava/lang/Object;
    const/4 v0, 0
    iput v0, p0, LStack;->size:I
    iput-object v1, p0, LStack;->data:[Ljava/lang/Object;

    return-void
.end method

.method public push(Ljava/lang/Object;)V
    .registers 4

    iget v1, p0, LStack;->size:I
    add-int/lit8 v1, v1, 1
    iput v1, p0, LStack;->size:I

    iget-object v0, p0, LStack;->data:[Ljava/lang/Object;
    iget v1, p0, LStack;->size:I
    sub-int/lit8 v1, v1, 1
    iget-object v2, p1, Ljava/lang/Object;->data:[Ljava/lang/Object;
    aput-object v2, v0, v1

    return-void
.end method

.method public pop()Ljava/lang/Object;
    .registers 4

    iget v1, p0, LStack;->size:I
    if-lez v1, :return_null

    iget v1, p0, LStack;->size:I
    add-int/lit8 v1, v1, -1
    iput v1, p0, LStack;->size:I

    iget-object v0, p0, LStack;->data:[Ljava/lang/Object;
    iget v1, p0, LStack;->size:I
    aget-object v0, v0, v1

    return-object v0

    :return_null
    const/4 v0, 0
    return-object v0
.end method
